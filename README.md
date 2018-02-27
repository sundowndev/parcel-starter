# What's inside ?

Fastshell + Webpack + Sass = 🔥

Fiercely quick front-end boilerplate and workflow with <a href="https://github.com/HosseinKarami/fastshell">Fastshell</a>, Javascript bundlers with <a href="https://github.com/webpack/webpack">Webpack</a> and CSS preprocessing with <a href="https://github.com/sass/sass">Sass</a>.

## Installation

Clone the repository

~~~
$ git clone https://github.com/SundownDEV/front-end-starter
~~~

Install dependencies and run the default gulp script

~~~
$ npm install
$ gulp
~~~

Open the project url `http://localhost:3000/`

## Overview

#### Directory structure
~~~
    |-- app
        |-- index.html
        |-- assets
            |-- css
            |-- js
    |-- src
        |-- scss
            |-- common.scss
        |-- js
            |-- app.js // Main application bundler
~~~

#### Minification and hot reloading

gulp-minify and gulp-cssnano minify css and js assets files, then Browser-sync reload the application server everytime you edit a scss/js file.

~~~ js
gulp.task('browser-sync', function() {
    browserSync.init(null, {
        server: {
            baseDir: "app"
        }
    });
});
~~~
