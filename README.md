# DataReachable Website

<div align="center">
	<img src="./images/logo.jpeg" />
	<br/>
	<div style="margin:auto">
		<span style="font-size:200%">DataReachable Website</span>
	</div>
</div>

# Description

This is the DataReachable Website specifications, it will include project structure introduction and how to setup and run the project.

# Project Structure

## Overview

```
ProjectSample/ .................... Project Folder
├─ package_backup/ ................ Package.json Backup Folder
├─ public/ ........................ Public Static Files Root Folder
│  ├─ favicon.ico ................. Project Favicon
│  ├─ icon.png .................... Project Icon
│  ├─ index.html .................. Project Production HTML File
│  └─ indexDev.html ............... Project Development HTML File
├─ src/ ........................... Project Root Folder
│  ├─ global.d.ts ................. Typescript Third-party Package Declaration File
│  ├─ index.tsx ................... Project Root File
│  ├─ _test_ ...................... Project Testing Folder
│  ├─ Assets/ ..................... Project Public Components Root Folder
│  │  └─ images ................... Project Images Root Folder
│  ├─ Components/ ................. Project Public Components Root Folder
│  │  ├─ index.ts ................. Unified Export Project Public Components File
│  │  └─ PublicComponentA/ ........ Project Public Component A Folder
│  │     ├─ index.tsx ............. Project Public Component A Entry File
│  │     └─ style.scss ............ Project Public Component A Style File
│  ├─ Util ........................ Project Util Folder
│  ├─ DefaultData ................. Project Component Default Data Folder
│  ├─ Constant/ ................... Project Resuable Style Root Folder
│  │  └─ 'name'.scss .............. Resuable Style File
│  ├─ Locales/ .................... Project Multilingual Configuration Folder
│  │  ├─ Translations ............. Resuable Style File
│  │  │  ├─ en .................... English Translations Folder
│  │  │  │  └─ translation.json ... English Translations file
│  │  │  └─ cn .................... Chinese Translations Folder
│  │  │     └─ translation.json ... Chinese Translations file
│  │  └─ i18n.ts .................. Multilingual Configuration file
│  ├─ PageLayouts/ ................ Project Page Layout Root Folder
│  │  ├─ index.ts ................. Unified Export Project Layouts File
│  │  └─ LayoutA/ ................. Project Layout A Folder
│  │     ├─ index.tsx ............. Project Public Layout A Entry File
│  │     └─ style.scss ............ Project Public Layout A Style File
│  ├─ Pages/ ...................... Project Pages Root Folder
│  │  ├─ index.ts ................. Unified Export Project Pages File
│  │  └─ PageA/ ................... Project Page A Folder
│  │     ├─ index.tsx ............. Project Page A Entry File
│  │     ├─ style.scss ............ Project Page A style
│  │     └─ Components/ ........... Project Page A Private Components Folder
│  │        └─ PrivateComponentA/ . Project Page A Private Component A Folder
│  │           ├─ index.tsx ....... Project Page A Private Component A Entry File
│  │           └─ style.scss ...... Project Page A Private Component A Style File
│  ├─ Route/ ...................... Route Root Folder
│  │  └─ index.tsx ................ Route Management Entry File
│  └─ Store/ ...................... Store Root Folder
│     ├─ rootReducer.ts ........... Root Reducer To Combine All Module Reducer
│     ├─ rootSaga.ts .............. Root Saga
│     ├─ rootStore.ts ............. Root Store
│     └─ moduleA/ ................. ModuleA Folder
│        ├─ types.ts .............. ModuleA Action Types File
│        ├─ actions.ts ............ ModuleA Actions File
│        ├─ reducer.ts ............ ModuleA Reducer File
│        └─ sagas.ts .............. ModuleA Asynchronous Request Function Management Saga File
├─ webpackConfig/ ................. Webpack Root Folder
│  ├─ webpack.common.js ........... Webpack General Configuration File
│  ├─ webpack.dev.js .............. Webpack Development Environment Packaging Configuration File
│  └─ webpack.prod.js ............. Webpack Production Environment Packaging Configuration File
├─ .babelrc ....................... Configure Presets And Plugins File
├─ .eslintignore .................. ESLint To Ignore Specific Files File
├─ .eslintrc.js ................... Typescript Syntax Detection Rules File
├─ .prettierrc.js ................. Code Formatting Style Rules File
├─ package.json ................... Project Configuration Information File
├─ postcss.config.js .............. Project Style Configuration File
└─ tsconfig.json .................. Typescript Compilation Rules File


```

## Public Folder

The public folder mainly contains some static files in the project, for example, the icon of the project, some local pictures and the root file of the project html in the project.

## Src Folder

The src folder mainly contains the entry file of the project, including all the style files, functional files, asynchronous request files and page routing management files in the project.

# Usage

## Local Environment Requirement

This project requires React with minimal version of 16.13.0 and thus, should install essential NPM packages prior to usage.

The following procedure assumes the node and npm have already been installed and are accessible from the commandline. For installation of node and npm, see [install node and npm](https://www.npmjs.com/get-npm).

## Install All The Necessary Package To The Project

Run the following command to install the packages:

```javascript
npm install
```

## Setting Up ESLint and Prettier To Work With This Project

For a good developer experience, it is useful to set the editor to automatically run ESLint's automatic repair commands when saving files.
To open your user and workspace settings, follow the following method:

On Windows/Linux - File > Preferences > Settings > Extensions > Scroll down and find "Edit in settings.json"

On macOS - Code > Preferences > Settings > Extensions > Scroll down and find "Edit in settings.json"

You can also open the Settings editor from the Command Palette (⇧⌘P) with Preferences: Open Settings or use the keyboard shortcut (⌘,), or see [User and Workspace Settings](https://code.visualstudio.com/docs/getstarted/settings) to get more information.

Now, You should have an open file to execute it. If you don’t want to format the file manually every time, you can also format it when saving. Therefore, you need to open the settings/preferences of Visual Studio Code users in JSON format and configure the following:

```javascript
{
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "editor.formatOnPaste": true,
  "editor.formatOnSave": true,
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript"
  ],
}
```

## Run The Project Demo

Enter the following command to run the demo:

```javascript
npm run start
```

## Project Specification

This is very important !! Before you start coding, please read the [Porject Specification](https://docs.datareachable.net/) carefully.