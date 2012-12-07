# Base SCSS Starter Framework

Version 1.5.3

## Contributors:

Matt Banks ( [@mattbanks](http://twitter.com/mattbanks) / [kernelcreativemedia.com](http://www.kernelcreativemedia.com) / [mattbanks.me](http://www.mattbanks.me) )

## Summary

Base Compass/SCSS framework for new websites.

## Usage

Code as you will. I use [CodeKit](http://incident57.com/codekit/) for Compass/SCSS compiling, but feel free to use whatever app or command line tool you prefer. [LiveReload](http://livereload.com/) and [Grunt](http://gruntjs.com/) are also great tools for compiling SCSS.

- Compile `scss/style.scss` to `css/style.css`
- Compile `js/plugins.js` to `js/plugins.min.js`
- Compile `js/main.js` to `js/main.min.js`
- ??
- Profit

### Features

1. Normalized stylesheet for cross-browser compatibility using Normalize.css version 2 (IE8+ only)
2. Easy to customize
3. Flexible grid from [Chris Coyier](https://twitter.com/chriscoyier)
4. Media Queries for mobile and tablets ready to populate
5. Compass & SCSS with plenty of mixins ready to go

### Changelog

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
* [SASS/SCSS](http://sass-lang.com/)
* [Compass](http://compass-style.org)
* [Don't Overthink It Grids](css-tricks.com/dont-overthink-it-grids/)
* [SCSS Media Query Mixins from Chris Coyier](http://css-tricks.com/snippets/css/media-queries-for-standard-devices/)
