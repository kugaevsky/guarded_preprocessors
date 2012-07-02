# Guarded preprocessors

Simple bundle to mock up web frontends with HAML/Coffee/Sass/Less

## Installing

__Environment:__ You must have installed `ruby` with `bundler` gem in your environment to use guarded_preprocessors.

1. `git clone git://github.com/kugaevsky/guarded_preprocessors.git` -- сlone (or download) repository to your machine
2. `cd guarded_preprocessors` change your working directory.
3. (Un)comment gems that you really (don't) need in `Gemfile`.
4. Run `bundle install` to install all dependencies.
5. Run `guard` command to watch files you modify.

## Usage 

Just run `guard` command in your working directory and edit files in your `source` directory.
All of them will be automagically compile in `html` directory of your project.

## Anatomy

* `source/` - directory for source files written in HAML/Coffee/Sass/Less
* `html/` - directory for compiled files in HTML/Javascript/CSS

Anyway, your can edit relative paths for each preprocessor in your `Guardfile`. 
Syntax is really very simple.

## Preprocessors

Right out the box you can use configured preprocessors

* __HAML__ – for HTML preprocessing
* __Coffescript__ – for Javascript preprocessing
* __Sass, Scss or LESS__ – for CSS preprocessing

## Thanks

To all guys that make frontend development faster and cleaner

* [Guard](https://github.com/guard)
* [HAML](http://haml.info/)
* [Coffescript](http://coffeescript.org/)
* [Sass](http://sass-lang.com/)
* [LESS](http://lesscss.org/)