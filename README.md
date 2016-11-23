# CastleCSS Core Files
![CastleCSS logo @CastleCss.com](https://www.doordarius.nl/castlecss-logo-250.png)

## CastleCSS Framework
The core files are part of the [CastleCSS Package](https://github.com/CastleCSS/castlecss)

## How to install
- Install via [npm](https://www.npmjs.com/): ```npm install castlecss-core```
- Require it in your own npm package
- Download or clone the package

## Updating files
CastleCSS is built so it's easy to update, you can just download make it your own as long as you don't ovewrite the core files. 

```npm update castlecss-core```

## Documentation and examples
You can find the documentation and examples at http://www.castlecss.com and [castlecss-docs](https://github.com/CastleCSS/castlecss-docs)


## Adjusting the variables
Because of the unique update-able setup of CastleCSS you need a seperate variable file to overwrite the default CastleCSS variables. There are a few ways to do this: 

- Use the [boilerplate](https://github.com/CastleCSS/castlecss-boilerplate/) which provides a variables.scss file
- Copy variables.scss from /node_modules/castlecss-core/sass/variables.scss into your own scss folder and include it into your main.scss
- Copy the example from the [documentation](http://castlecss.com/variables.html) into your own variables.scss and include it into your main.scss

## Basic structure
The basis structure for your website should look similar like this:

```
| Project directory/
|
|-- node_modules/
| | -- castlecss-core/
| | --castlecss-buttons/
| | --castlecss-notifications/
| |
|-- scss/
| |-- main.scss
| |-- variables.scss
| |
|-- img/
|-- dist/
| |-- styles.min.css
| |-- styles.min.map
| |
|-- index.html
|-- Gruntfile.js
|-- package.json
```

### main.scss
Your main.scss should have the following set-up:

```
/* 	CastleCSS Core variables */
@import "node_modules/castlecss-core/sass/variables";

/* 	Your variables */
@import "variables";

/* 	Remaining Core files and other CastleCSS modules */
@import "node_modules/castlecss-core/sass/main";
@import "node_modules/castlecss-buttons/sass/main";
@import "node_modules/castlecss-notifications/sass/main";

/* Include your own files below this line
   -------------------------------------- */



/* --------------------------------------
   Include your own files above this line */

@import "node_modules/castlecss-core/sass/base/utility";
@import "node_modules/castlecss-core/sass/base/utility_spacers";
```
