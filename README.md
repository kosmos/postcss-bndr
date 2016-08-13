Postcss-bndr
=========

Postcss plugin which adds the specified string to the end of the CSS file.

## Installation

  npm install postcss-bndr --save-dev

## Usage

    var gulp         = require('gulp');
    var postcss      = require('gulp-postcss');
    var bndrplugin   = require('postcss-bndr');

    var processors = [
    bndrplugin({
        message: 'Сайт створенно із використанняс магії! :)'
    })];

    gulp.task('postcss', function(){
    gulp.src('src/style.css')
        .pipe(postcss(processors))
        .pipe(gulp.dest('dest'));
    });

## Options

    message - A string with a message that should be added to the generating CSS file.

## Release History

* 0.1.0 Initial release
