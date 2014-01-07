# Base SCSS Starter Framework

Version 2.0.3

## Author:

Matt Banks ( [@mattbanks](http://twitter.com/mattbanks) / [kernelcreativemedia.com](http://www.kernelcreativemedia.com) / [mattbanks.me](http://www.mattbanks.me) )

## Summary

Base Compass/SCSS framework for new websites. Uses Compass/SCSS, HTML5 Boilerplate 4 with Modernizr and Normalize.css, and Grunt for all tasks.

## Usage

The theme is setup to use [Grunt](http://gruntjs.com/) to compile Compass/SCSS, lint, concatenate and minify JavaScript (with source maps), optimize images, and [LiveReload](http://livereload.com/) the browser (with extension), with flexibility to add any additional tasks via the Gruntfile. Alternatively, you can use [CodeKit](http://incident57.com/codekit/) or whatever else you prefer to compile the SCSS and manage the JavaScript.

Open the project directory in terminal and run `npm install` to pull in all Grunt dependencies. Run `grunt` to execute tasks. Code as you will. If you have the LiveReload browser extension, it will reload after any SCSS or JS changes. To optimize images, run `grunt imagemin`.

- Compile `assets/scss/style.scss` to `style.css` (all paths defined in config.rb for Compass)
- Compile `assets/scss/editor-style.scss` to `editor-style.css`
- Concatenate and minify plugins in `assets/js/vender` and `assets/js/source/plugins.js` to `assets/js/plugins.min.js`
- Minify `assets/js/source/main.js` to `assets/js/main.min.js`
- ??
- Profit

To concatenate and minify your jQuery plugins, add them to the `assets/js/vendor` directory and add the `js` filename and path to the `Gruntfile` `uglify` task. Previous versions of the starter theme automatically pulled all plugins in the `vendor` directory, but this has changed to allow more granular control and for managing plugins and assets with bower.

### Bower

Supports [bower](https://github.com/bower/bower) to install and manage JavaScript dependencies in the `assets/js/vendor` folder.

### Deployment

The theme includes deployments via [grunt-rsync](https://github.com/jedrichards/grunt-rsync). The Gruntfile includes setups for staging and production - edit your paths and host, then run `grunt rsync:staging` or `grunt rsync:production` to deploy your files via rsync.

### Features

1. Normalized stylesheet for cross-browser compatibility using Normalize.css version 2 (IE8+ only)
2. Easy to customize
3. Flexible grid from [Chris Coyier](https://twitter.com/chriscoyier)
4. Media Queries for mobile and tablets ready to populate
5. Compass & SCSS with plenty of mixins ready to go

![dependencies](https://david-dm.org/mattbanks/Base-SCSS-Project-Framework.png)

### Changelog

#### Version 2.0.3

* update grunt dependencies
* update spacing in functions

#### Version 2.0.2

* update grunt dependencies
* update deployment info to fit new rsyncwrapper options

#### Version 2.0.1

* update grunt dependencies
* switch to load-grunt-tasks for loading everything
* restructure deploy task based on grunt-rsync updates

#### Version 2.0.0

* reorganize code in `assets` folder for fonts, images, js and scss
* setup Gruntfile to use Grunt for all compiling, concatenation and minification
* add deployments via rsync
* add bower support with `.bowerrc`
* general code cleanup

#### Version 1.5.4

* Add grid column sizes I typically use, general code cleanup

#### Version 1.5.3

* Fix text selection bg and color not pulling from variables

#### Version 1.5.2

* Fixed broken html tag comment
* Fixed broken modernizr link (`/js/vendor/` instead of `/js/lib/`)

#### Version 1.5.1

* Move border-box from `_grid.scss` to `_global.scss`
* Add border-box support for pseudo elements, because it makes the world a better place

#### Version 1.5

* Updated to HTML5 Boilerplate 4
* Updated to Normalize.css 2
* Updated to Modernizr 2.6.2
* Updated to jQuery 1.8.3
* Renamed jquery.functions.js to main.js
* Add flexible grid SCSS
* Include @media bubbling mixins, [via Chris Coyier](http://css-tricks.com/snippets/css/media-queries-for-standard-devices/)
* Other bug fixes and changes

#### Version 1.1

* add compass via config.rb
* add compass mixins in style.scss
* remove mixins that compass has by default
* change directory structure

#### Version 1.0

* initial version

### Credits / Projects Utilized

* [HTML5 Boilerplate](http://html5boilerplate.com)
* [Normalize.css](http://necolas.github.com/normalize.css))
* [SASS / SCSS](http://sass-lang.com/)
* [Compass](http://compass-style.org)
* [Don't Overthink It Grids](css-tricks.com/dont-overthink-it-grids/)
* [SCSS Media Query Mixins from Chris Coyier](http://css-tricks.com/snippets/css/media-queries-for-standard-devices/)
* [Grunt](http://gruntjs.com/)
* [Bower](https://github.com/bower/bower)
