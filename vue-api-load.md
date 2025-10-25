# Vue API Load

## Reasoning

The vanishing pages issues we've experienced start when the components are re-opened and the data needs to be reloaded. These issues happen because vue is expecting that data to be **immediately** available, but since the data has to be rendered and some html elements need to be fetched and rendered (images), it will cause a render error for the component.

## Fix

We need to add a new variable called `loaded` and set it as false by default and then set the value to `true` when the data is loaded.

We also need to wrap the parts that uses the incoming wordpress data inside a tag that uses the `v-if` directive and it should verify if value of `loaded` is `true`.

> [!NOTE]
> The wrapper doesn't need to be a ul, it can be some other container tag, like section, article, div or span.

```js
<script setup>
import { onMounted, ref } from "vue";
let wordpress = ref([]);

let loaded = ref(false);

let fetchData = async () => {
  try {
    const response = await fetch("https://ngy.582mi.com/headless/wp-json/wp/v2/posts");
    if (!response.ok) {
      throw new Error(`HTTP error! status: ${response.status}`);
    }
    const data = await response.json();
    wordpress.value = data;

    loaded.value = true;

  } catch (error) {
    console.error(error);
  }
};
onMounted(() => {
  fetchData();
});
</script>

<template>
  <section>
    <h1>WP API Test</h1>

    <div v-if="!loaded">
      Loading...
    </div>
    <ul v-if="loaded">

      <li v-for="item in wordpress" :key="item.id">
        {{ item }}
      </li>
    </ul>
  </section>
</template>
```