# Magento-Bootstrap theme for Mage_Lite

This project is a fork of [Magento-Bootstrap theme](https://github.com/EcomDev/mbootstrap) modified specifically for use with Mage_Lite. It is a theme package fully based on Twitter Bootstrap framework.

## Status:

Current version: Alpha

## Assets

* Bootstrap v2.3.1
* Font Awesome v3.0.2
* HTML5 support
* Microdata support (schema.org)

## How to install

1. `modman clone git@github.com:colinmollenhour/mbootstrap-lite.git mboostrap`
2. Open Admin Panel
    * go to **System -> Configuration**
    * open **Design** tab on left sidebar
    * open **Package** section
    * write "bootstrap" in *Current Package Name* field
    * press "Save Config" button
    * open **Developer** tab on left sidebar
    * open **Template Settings** section
    * change **Allow Symlinks** to **Yes**
    * press "Save Config" button
3. Refresh front-end page and enjoy

## How to use

Really it is very-very easy to use :)

Develop process as usual for Magento theme (more about front-end develope for Magento you can see on [Designer's Guide To Magento](http://www.magentocommerce.com/design_guide/articles/working-with-magento-themes))

### Create your theme based on Magento-Bootstrap theme

You need create custom theme based on Magento-Bootstrap theme. 
After `git clone` command you will have next folder hierarchy:

```
.
├── app
│   └── design
│       └── frontend
│           └── bootstrap
│               └── default
├── skin
│   └── frontend
│       └── bootstrap
│           └── default
```

So you need create new theme in **bootstrap** package

**Example**
```
.
├── app
│   └── design
│       └── frontend
│           └── bootstrap
│               ├── default
│               └── custom-theme
├── skin
│   └── frontend
│       └── bootstrap
│           ├── default
│           └── custom-theme
```

That's it!
Now you can develop your custom theme based on Magento-Bootstrap theme

(i) don`t forget enter your just created theme name (in example it is *custom-theme*) 
at Admin Panel (System -> Configuration -> General -> Design tab -> Themes section -> Default field)

## Skin folder structure description

Open *magento/skin/frontend/bootstrap/default* path

```
.
├── Makefile              -- Script file with *compile* less to css and *watch* file system changes commands. Open it and read *How to use*
├── bootstrap             -- Bootstrap framework source files
├── css                   -- Theme css files compile there
├── fonts
│   └── Font-Awesome      -- The iconic font designed for use with Twitter Bootstrap
├── images
├── js
├── less                  -- Theme less files
└── watcher.js            -- More powerful watch program for OSX (with lessc, watchr, growl). Open it and read *Requirements* for use

```

## Developer tools

Magento-Bootstrap theme contains also developers tools:
* run *less to css* compile
* run file system watching program and compile *less to css* automatically

For more information go *magento/skin/frontend/bootstrap/default/* folder and read *Makefile* file

### Requirements

1. Node.js                              -- Open http://nodejs.org and install latest Node.js version
2. Bootstrap framework install          -- Open *magento/skin/frontend/default/bootstrap* and run `$ npm install` command in terminal


## Special Thanks

Special thanks to the guys at EcomDev for your work on Magento-Bootstrap theme.

<a href="http://www.ecomdev.org/services/magento-development?utm_source=github&utm_medium=logo&utm_campaign=github">![EcomDev](http://www.ecomdev.org/wp-content/themes/ecomdev/images/logo.png)</a>
