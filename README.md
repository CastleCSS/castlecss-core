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

## Documentation and examples
You can find the documentation and examples at http://www.castlecss.com and [castlecss-docs](https://github.com/CastleCSS/castlecss-buttons)

## Setup
Your project should have a setup similair to this (included in the [Full CastleCSS Package](https://github.com/CastleCSS/castlecss)):
With this you make sure your own variables overwrite the castle-core variables and your setup is still updatable.

```
| Your project/
|
|-- scss/ 
| |-- /* Custom project specific scss files here */
| |-- Main.scss
| |
|-- node_modules/
| | 
| | /*	CastleCSS files included automatically here */
| | castlecss-core/
| | castlecss-buttons/
| | castlecss-etc ;)/
```

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
