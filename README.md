# Front-end starter

Simple front-end starter using sass preprocessor with gulp. **You need to install npm.**

## Installation

~~~
$ npm install
$ gulp watch
~~~

## Usage

Include sass files in common.sass
~~~ sass
@import '_reset';
@import '_conf';
@import '_global';
@import '_header';
@import '_menu';
@import '_about';
@import '_footer';
~~~

Use _conf.sass to initialize colors, fonts, and transitions
~~~ sass
$containerWidth: 117rem;

// Colors

$color1: #ff2b4a;
$color2: #835aeb;
$color3: #002453;
$color4: #10c6fc;
$color5: #64cbc0;

$textColor: black;
$firstDegrade: #7a6b7b;
$secondDegrade: #30697d;

// Fonts

$fontFamilyText: "Roboto", Arial;
$fontFamilyTitle: "Raleway", Arial;

// Conf vars

$transition: ease-out .4s;

// Mixins

@mixin backgroundImage($image) {
  background: url('../../images/#{$image}')
}
~~~
