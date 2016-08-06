# CastleCSS Core Files
![CastleCSS logo @CastleCss.com](https://www.doordarius.nl/castlecss-logo-250.png)

## CastleCSS Framework
The core files are part of the [Full CastleCSS Package](https://github.com/CastleCSS/castlecss)


## How to install
- Install via [NPM](https://www.npmjs.com/): ```npm install castlecss-core```
- Require it in your own NPMJS package
- Download or clone the package

## Updating files
CastleCSS is built so it's easy to update, you can just download make it your own as long as you don't ovewrite the core files. 

```npm update castlecss-core```

## Setup
Your project should have a setup similair to this (included in the [Full CastleCSS Package](https://github.com/CastleCSS/castlecss).):
With this you make sure your own variables overwrite the castle-core variables and your setup is still updatable.


    | Your project/
    |-- sass/ 
    |  |-- Custom project specific files here
    |  |-- Main.scss //include castlecss main.scss files here first, your project specific files after that
    |  |
    |  |-- node_modules/ //CastleCSS files are automatically installed here
    |  |  |
    |  |  | castlecss-core/
    |  |  |  |
    |  |  |  |-- sass/
    |  |  |  |  |-- main.scss - include all your other SCSS files
    |  |  |  |
    |  |  |  |-- base/
    |  |  |  |  |-- reset.scss - set browser defaults to zero/none so nothing weird happends in different browsers
    |  |  |  |  |-- variables.scss - Variables for the grid, fonts, utility, etc
    |  |  |  |  |-- defaults.scss - Set default web settings
    |  |  |  |  |-- mixins.scss - Small but handy collection of mixins to use
    |  |  |  |  |-- utility.scss - Utility classes
    |  |  |  |  |-- utility_spacers.scss - Utility padding / margin classes
    |  |  |  |
    |  |  |  |-- layout/
    |  |  |  |  |--  grid.scss - *Flexbox scss grid with floating fallback*
    |  |  |  |  |--  static_files.scss - *Static files like containers*

### Main.scss
Your main.scss should have a setup similair to this (included in the [Full CastleCSS Package](https://github.com/CastleCSS/castlecss)):

```
/*  core variable files */
@import "node_modules/castlecss-core/sass/variables";
/*  Your own variables so they overwrite the core */
@import "variables";
/*  rest of core files */
@import "node_modules/castlecss-core/sass/main";
 
/*  Include your own files below this line
    --------------------------------------
*/
```
