---
layout: default
title: Environment Setup
nav_order: 2
---

# Environment Setup
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

----

### Gulp

We are using gulp to compile are SASS file into CSS. dotCMS current does have a SASS compiler but it has proven to be unreliable at times. Also, if the compiler finds an error in the SASS files, it will render a blank css file rather then leave the current compiled css live. This means that the site would load a blank page until the issue is fixed. We are using npm to install Gulp and serve the Foundation 6 sass files. Compiling offline is a safer way so that the process of development continues without possibly break the site. If the dotCMS compiler situation addressed, we will upload the sass files to have dotCMS compile the css and remove the local compiler css for production use.


### Gulp Installation

The follow commands are used to install the tools used in this project. You must be in the root directory when installing these tools. Run the follow command to install all tools and dependancies:
```
$ npm install
```

If you and a tool to the project, please don't forget to add it to the package.json file. Run the follow command when installing new tools or dependencies:
```
$ npm install --save { package }
```
OR
```
$ npm install --save-dev { package }
```

#### Using Gulp
- SASS Compile Foundation (Not Minified): `gulp app`
- SASS Compile Taylor Styles (Not Minified): `gulp style`
- SASS Compile while working (Not Minified): `gulp watch`
- SASS Compile and Minify: `gulp -task`
