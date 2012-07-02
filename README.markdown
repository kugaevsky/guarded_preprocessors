# Guarded preprocessors

Simple way to mock up web frontends with HAML/Coffee/Sass/Less

## Installing

You must have installed `ruby` with `bundler` gem in your environment to use this template

1. Clone (or download) repository to your machine
2. `cd` in cloned repository directory
3. Comment/uncomment gems that you really (don't) need in `Gemfile`
4. Run `bundle install`
5. Run `guard` command

## Usage 

Just run `guard` command in your working directory and edit files in your `source` directory.
All of them will be automagically compile in `html` directory of your project

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