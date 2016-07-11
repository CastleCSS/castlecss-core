# CastleCSS Core Files

## What is CastleCSS?
CastleCSS a mobile first SCSS framework with modular building blocks for the web

## What is different between CastleCSS and other frameworks?
Unlike other Frameworks we don't include *everything*, you don't need everthing :): but only what you need. 
You pick what you want to use. The core is a way to kickstart your website with the basic files and philosophy we believe in.

Our philosophy is mobile first, self explanatory code code and breakpoints. On the other hand we want to be able to keep you up to date with the latest version of CastleCSS, this is possible if you overwrite the defaults the way you're supposed to.

### Breakpoint CSS
We don't believe in classes like *laptop* or *small* and other classes but we define everything with **b{breakpoint}** this makes everything readable and since we use this throughout the whole framework everything feels familiar when you use it for a while. Whether it's for grid, utility classes, hiding, showing. It all starts with **b{breakpoint}**

## What's included
CastleCSS Core has the following basic files to kickstart your website:

- main - *include all your other SCSS files*
- reset - *set browser defaults to zero/none so nothing weird happends in different browsers*
- variables - *Variables for the grid, fonts, utility, etc*
- grid - *Flexbox scss grid with floating fallback*
- defaults - *Set default web settings*
- mixins - *Small but handy collection of mixins to use*
- utility - *Utility classes*
- utility_spacers - *Utility padding / margin classes*

## How to install
You can install castle css with NPM in your sass folder:

	npm i castlecss-core
	
### How to update
Type the following to check for updates in your sass folder:
	
	npm outdated

Then type the following to npm update

	npm update

If you didn't alter the core files it will now update

# SCSS folder structure and overwriting the CastleCSS defaults
Of course you want to be able to set your own variables and other classes. To do this: make your own custom folder outside of node modules and include the files. The ideal structure of your SASS folder should be the following:

	| Your project
	| -- sass/ //your custom scss goes here
	| -- | main.scss //include your own SCSS files and /node_modules/castlecss-core/main.scss here
	| -- | node_modules/ //CastleCSS files are automatically installed here
	| -- | -- castlecss-core/
	| -- | -- | sass 
