# Guarded preprocessors     [![endorse](http://api.coderwall.com/kugaevsky/endorsecount.png)](http://coderwall.com/kugaevsky)

Simple bundle to mock up web frontends with HAML/Coffee/Sass/Less.
Autocompiles your files on every save and refreshes browser without `⌘+R` or `F5`

## Installing

__Environment:__ You must have installed `ruby` with `bundler` gem in your environment to use guarded_preprocessors.

1. `git clone git://github.com/kugaevsky/guarded_preprocessors.git` – сlone (or download) repository to your machine
2. `cd guarded_preprocessors` change your working directory.
3. Uncomment notification gems that you really need in `Gemfile`.
4. Uncomment notification instructions in `Guardfile`.
5. Run `bundle install` to install all dependencies.
6. Run `guard` command to watch files you modify.

## Usage 

Just run `guard` command in your working directory and edit files in your `source` directory.
All of them will be automagically compile in `html` directory of your project.

## Anatomy

* `source/` - directory for source files written in HAML/Coffee/Sass/Less
* `html/` - directory for compiled files in HTML/Javascript/CSS

Anyway, your can edit relative paths for each preprocessor in your `Guardfile`. Syntax is really very simple. 
Just redefine paths hash.
`PATHS = { :in => 'source', :out => 'html' }`

## Preprocessors

Right out the box you can use configured preprocessors

* __HAML__ – for HTML preprocessing
* __Coffescript__ – for Javascript preprocessing
* __Sass, Scss or LESS__ – for CSS preprocessing

## Notifications

Your can configure system notifications for guarded files compilation. Follow instructions in `Gemfile`. Just uncomment gem lines for your OS. And install notification software if needed.

* **MacOS users:** Growl notifications – [GrowlNotify](http://growl.info/extras.php#growlnotify)
* **Linix users:** Libnotify notifications – install `libnotify-bin` package with your favorite package manager.
* **Windows users:** Notifu notifications – [Notifu](http://www.paralint.com/projects/notifu/)

## LiveReload

LiveReload can autorefresh page in your browser on every file modification. To use this incredible feature just

1. Install extension for your browser (Safari, Chrome, Firefox supported) from [livereload extension page](http://feedback.livereload.com/knowledgebase/articles/86242-how-do-i-install-and-use-the-browser-extensions-).
2. Open your page in browser and turn on `LiveReload` by clicking on extension icon.
3. **NB Chrome users:** if you work without any web-server (opened file URL looks something like `file:///my-perfect-page.html`), you have to grant permissions for extensions to work with local files in Chrome. Go to extension management page `chrome://chrome/extensions/` and check `Allow access to file URLs` option below LiveReload extension.

That's all. Just save your file and it will be compiled and rendered in your browser in a moment.

**TIP**
If you want more information about livereload connection to your browser add `?LR-verbose` to your file URL.

## Thanks

To all guys that make frontend development faster and cleaner

* [Guard](https://github.com/guard)
* [HAML](http://haml.info/)
* [Coffescript](http://coffeescript.org/)
* [Sass](http://sass-lang.com/)
* [LESS](http://lesscss.org/)
* [LiveReload](http://livereload.com/)


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/kugaevsky/guarded_preprocessors/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

