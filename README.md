# Web 5: Web Applications

## UPDATES (Oct 18th)

Everyone should be starting **BOTH** of your sites on vue now. Your task is basically to transcribe the basic HTML structure from your figma planning.

Use images from your work or clients if you have them (please resize to max size you intend to use)

> [!TIP]
> If you are missing images, placeholder images from <https://placehold.co/> or other online services are acceptable, but not ideeal.

Make sure you test things out (and commit) on your sandbox vue project for any of the techniques I’ve shown in class or if you want to remind yourself how to do some of the vue components and setup.

> [!IMPORTANT]
> I want clean small commits for everything you do for your portfolio and your client vue projects.

### What you should have in your vue projects

- import main.css (or name it appropriately for your client) into the main.js
- this css file should at the minimum have css reset and you can also set up the css variables I showed in class so you can use your main colors everywhere and change it later
- set up views in a view folder (using your html structure)
- set up routes that uses those views
- adjust your code if you need to use any scrolling features I showed in class.
- no need to connect to wordpress for now, you can hardcode some sample details into the views so we can see it's functional and if any tags needs to be change before we start pulling data from wordpress.
- components at this stage are not entirely necessary yet, we can split your code into components later, but if some of you want to do it right away, you can.

### USEFUL LINKS

- [Scroll & fancy css demos](https://github.com/ngyvc?tab=repositories)
- [Sandbox](https://sandbox.582multi.media/)
- [Web 5 notes](https://github.com/582Multimedia/web5-web-apps)
- [Old web4 notes](https://github.com/582Multimedia/web4-db-cms)

### Commands you might need

#### windows command fix

```cmd
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```

#### git user info setup and pull.rebase

```bash
git config --global user.name "Your Name"
git config --global user.email "12345678@edu.vaniercollege.qc.ca"
git config --global pull.rebase true
```

#### vue - create new project

```bash
npm create vue@latest
```

vue options we need:

- router
- pinia
- eslint
- prettier

## Course Plan

| Week | Dates | Due (portfolio) | Due (client) | Plan |
| --- | --- | --- | --- | --- |
| 01 | Aug 27 / 29 |  | wow nothing due! I guarantee you it will be the only week | course intro + immediate 3rd deg grilling |
| 02 | Sept 3 / 5 | Catagorized list of **_all_** multimedia projects you have worked on | | Git + Inspo / wireframing for portfolio |
| 03 | Sept 10 / 12 | Complete wireframe & portfolio requirements | Lockdown client | CSS Review - Begin figma for portfolio |
| 04 | Sept 17 / 19| Fully functional figma | Client Questionnaire | WP + Vue Review + Begin vue for portfolio |
| 05 | Sept 24 / 26 | Basic vue + wordpress + custom post types (CPT) setup | Client wireframe | Advanced vue templating |
| 06 | Oct 1 / 3 | Add adv vue templating | Client Figma | Advanced css 1 |
| 07 | Oct 8 / 10 | Add adv css | Client Vue + wordpress + CPT | Advanced css 2 |
| 08 | Oct 15 / 17 (Midpoint) | Protfolio version 1 | --- | Portfolio critiques #1 |
| 09 | Oct 22 / 24 | --- | Client feedback #1 | *** |
| 10 | Oct 29 / 31 (Workshop) | --- | --- | Updates |
| 11 | Nov 5 / 7 |  Protfolio version 2 | --- | Portfolio critiques #2 |
| 12 | Nov 14 / 19 | --- | Client feedback #2 | Case study Introduction |
| 13 | Nov 21 / 26 | --- | --- | Plan |
| 14 | Nov 28 / Dec 3 | --- | Client feedback #3 | Plan |
| 15 | Dec 5 / 10 | --- | --- | Presentations |

- :grimacing: [Vue Recap](./vue.md)
- playground

## Projects

### - Web Portfolio

> [!IMPORTANT]
> Pick your domain name **_as soon as possible_**.

### - Client Project

> [!IMPORTANT]
> Find a client **_as soon as possible_**.

### -  Case Study

### -  Social Media

### -  Weekly git reviews
