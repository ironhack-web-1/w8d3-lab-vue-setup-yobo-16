![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# LAB | Vue.js Setup

## Introduction

In this lab, you'll start exploring how Vue.js works and how to create a project using this web development framework.

Your goals for this lab will be the following:

- Installing the Vue.js CLI on your computer
- Creating a new Vue project with a specific set of configurations
- Creating a new Vue component inside your project and showing it on the home screen
- Showing data from your JavaScript inside your HTML

We'll be following the official Vue.js guide for most of this lab.

## Setup

- Fork this repo
- Clone this repo
- Open the LAB and start:

  ```bash
  $ cd lab-vue-setup
  ```

## Submission

- Upon completion, run the following commands:

  ```bash
  git add .
  git commit -m "done"
  git push origin main # or master if you are working from a master
  ```

## Getting Started

<!-- Installing the CLI -->

1. The first step before creating your first Vue project will be to **install the CLI**. You only need to take this step once on your computer.

You can find the instructions [in this link](https://cli.vuejs.org/guide/installation.html). Remember to add the `-g` command in order to install Vue on your computer instead of just inside a specific folder.

If you're working on Mac, remember you'll need to add the keyword "sudo" before the command in order for it to work.

<!-- ## Create a new Vue project -->

2. Next, you will proceed to create a new project. Creating a new project on Vue is as simple as inserting a command on your console once you've installed the CLI globally. You can see the exact steps to follow [in this link](https://cli.vuejs.org/guide/installation.html).

Once you're creating a new project, you'll be able to choose which features you want. In this case, we want you to choose a few features manually:

- Babel
- Linter / Formatter + Prettier

We also want you to create a Vue 3 project. If you have any questions, the documentation is your best friend!

## Instructions

### Iteration 0 | Remove scaffolder

Remove the folders the following files in order to start from the scratch:

- folder `components`
- folder `assets`
- file `App.vue`

Create an empty file named App.vue with the following content: 

```
<template>
  <div>
    Vue 3!
  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>

<style>

</style>

```

You should have something like this:
![image](https://user-images.githubusercontent.com/108828282/186917079-bfc29e92-0d22-43ba-82cc-3aec62695c14.png)


### Iteration 1 | Create a new Vue component inside your project and show it on the home screen

Have you created your first project yet? Great! Now you'll start navigating inside the project's structure.

In order to make your life easier, we recommend you to install the [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) extension. It will help you create new components and add functionalities in an easier way.

Once you've created your new project and navigated inside the folder the CLI has created, you can now create your first Vue component!

Here's a helpful guide in case you're stuck: [How to create a Vue component](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/Vue_first_component).

Pro tip: if you use the Vetur extension, you just need to write "vue" inside your .vue file and choose the appropriate template to get a basic structure.

Once you've created your new component, we want to show it inside the App.vue file. We've already seen in class how to do that, but [here's a step-by-step guide](https://flaviocopes.com/vue-import-component/) that'll help you with this task.

Instructions:

- Create a component named `About.vue`
- Import the component in App.vue
- "Require" the component in the App component (in the `components` property )
- Use it in you template

### Iteration 2 | Showing data from your JavaScript inside your HTML

Now that you have your new component, we're going to practice how to link the elements inside the `<script>` with our `<template>`.

For this, you'll need to understand `Text Interpolation`. If you need a refresher about it, [here's the link to the official documentation](https://vuejs.org/guide/essentials/template-syntax.html#text-interpolation).

Instructions:

- Create a variable in your compontent's data property named `aboutMe` with a lorem ipsum text.
- Use the new variable in the component's template

You should see the text in the browser!
