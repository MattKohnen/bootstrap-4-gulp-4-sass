# Bootstrap 4 + Gulp 4 + SASS Boilerplate
A [Bootstrap](https://getbootstrap.com/) v4 boilerplate with [Sass](http://sass-lang.com/), concatenation, minification, [Browsersync](https://www.browsersync.io/), hot reloading and sourcemaps all managed by [Gulp](https://gulpjs.com/) v.4.

![bootstrap logo](https://user-images.githubusercontent.com/10498583/31125543-e2a88c2c-a848-11e7-87b0-d20ea38d41d0.jpg)
![sass logo](https://user-images.githubusercontent.com/10498583/31125541-e2a732e6-a848-11e7-959d-7d7b0c138124.jpg)
![gulp logo](https://user-images.githubusercontent.com/10498583/31125542-e2a78b88-a848-11e7-8ac5-c396f46e811f.jpg)
![browsersync logo](https://user-images.githubusercontent.com/10498583/31125540-e2a6eed0-a848-11e7-817a-69c5619f772a.jpg)

## Quick Start
### 1. Clone this Repo
`git clone https://github.com/MattKohnen/bootstrap-4-gulp-4-sass`

### 2. Navigate into the Repo Directory
`cd bootstrap-4-gulp-4-sass`

### 3. Install All Node Packages
`npm install`

### 4. Get Started
* `gulp` - starts localhost server with browser-sync, watches HTML, Sass, JS with hot reloading
* `gulp --prod` - minify CSS/JS and builds your app into the dist directory, ready for production

## Requirements
This project requires you have [nodejs](https://nodejs.org/en/) with [npm](https://www.npmjs.com/get-npm) installed.
This project requires you have a global installation of [gulp](http://gulpjs.com/).
```
# Install gulp globally
npm install -g gulp
```

## Gulp Commands
```
gulp
```

The default `gulp` command:
* Places the output of all Sass files into main.css and all JS files are concatenated into index.js
* Starts a local Browsersync server that serves your files in the browser
* Reloads the current page when changing HTML, Sass and JS files

Note that on *very rare* occasions changes might not reflect in the browser. 
In that case, try restarting the *server*.

You can access the development server with other devices on the same network. 
Go to the "External" address specified by Browsersync (see the terminal) in the web browser of your device.

```
gulp --prod
```

The default `gulp` command with the `--prod` flag passed in creates a production version of the CSS and JS, ready to be deployed.
It cleans the old "dist" directory as well as minifies and renames CSS/JS assets.

## Overwriting Bootstrap Sass Variables
You can leverage Bootstrap Sass via the **src/styles/1-vendor-overrides/bootstrap-overrides** directory:
* You can overwrite specific Bootstrap Sass variables via **_override-defaults.scss**
* You can extend existing Bootstrap classes with new classes via **_extend-classes.scss**
* You can use Bootstrap mixins via **_use-mixins.scss**

**Look inside of each of the above 3 files for examples.**
