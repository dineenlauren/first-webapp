# first-webapp

> A Vue.js project

# Build Setup

## **Setting Up Your Development Environment**

### Install Vue-CLI

1. Run the following command within your CLI:
   
   `npm install -g vue-cli`

2. Once installation is complete, check which version was installed by running:

   `vue --version`

   *If the installation was successful, you will see the version number displayed.*
### Install Webpack
1. Change to your preferred project directory location and run the following command:

   `vue init webpack [project-name]`

   *Do not include the brackets `[ ]` - replace "project-name" with the name of your project directory.*

2. Answer the following questions for set-up:
   ``` bash
   $ vue init webpack project-name

   ? Project name (project-name)
   ? Project name project-name
   ? Project description (A Vue.js project)
   ? Project description A Vue.js project
   ? Author (Name <GitHubname@users.noreply.github.com>)
   ? Author Name <GitHub@users.noreply.github.com>
   ? Vue build runtime
   ? Install vue-router? (Y/n) n
   ? Install vue-router? No
   ? Use ESLint to lint your code? (Y/n) n
   ? Use ESLint to lint your code? No
   ? Set up unit tests (Y/n) n
   ? Set up unit tests No
   ? Setup e2e tests with Nightwatch? (Y/n) n
   ? Setup e2e tests with Nightwatch? No

    Project initialization finished!
    ========================

   Documentation can be found at https://vuejs-templates.github.io/webpack
   ```
   You have now created a new directory called `project-name/` Change into this directory with `cd project-name/`

### Install Dependencies

1. Install Node.js. Run the following command:

   `npm install`

   *You should now have a node_modules/ directory in the root of `project-name/`*

## **Running the Development Server**
1. Run the following command:

   `npm run dev`

2. Your applicaton can now be viewed at http://localhost:8080
3. To Exit your Application from the CLI hit `CTL-C`

### Insert Your Own Content

1. **Modify the `HelloWorld` Component** : Open `src/components/HelloWorld.vue` in your code editor.

2. Change the template code to:
   ``` HTML
    <template>
        <div class="hello">
            <h1>{{ msg }}</h1>
            <h2>2 Things that are difficult in JavaScript</h2>
            <ol>
                <li>naming things</li>
                <li>recursion</li>
                <li>off-by-one errors</li>
            </ol>
        </div>
    </template>
   ```
3. Now you can make your changes between the `<template>` tags within the HelloWorld.vue files.

## **Deploying the App**

### Create Your Repository

1. Create a new Repository on GitHub
   * You do not need to add a README file as you already have it in your project directory
2. Go back to your CLI and create this new repository within your `project-name/` directory. Run the following commands:
   ``` bash
   git init
   git add -A
   git init
   git commit -m "commit message"
   git remote add origin git@github.com:yourGitHub/project-name.git
   git push -u origin master
   ```
### Configure Webpack

1. Webpack currently builds your files in the `dis/` directory.  Change this to the `docs/` directory by:
   * Within the `config/index.js` file, change all instances of `dis/` to `docs/`
   * Remove the "`/`" from `assetsPublicPath:'/'`

### Build the Code
1. Run the **build command**:
   
   `npm run build`
   
   *Your files will now be minified and built to the `docs/` folder*

### Deploy to Github Pages
1. Go to your GitHub Repository for `project-name` and navigate to **"Settings"** 
2. Under **"GitHub Page"** change your source to **master branch /docs folder**

**You can now view your project at your GitHub URL for that repository.**

# Commands Cheat Sheet
``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
