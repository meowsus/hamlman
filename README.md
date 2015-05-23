# Hamlman

A Haml-based [Middleman](http://middlemanapp.com) starter project template.

## Installation

- [Install Middleman](https://middlemanapp.com/basics/install/)
- Download the Hamlman project template
    + `git clone git@github.com:meowsus/hamlman ~/.middleman/hamlman`
- Initialize a new Hamlman project
    + `middleman init my_project --template=hamlman`

## Updating

Once Hamlman is downloaded to your `~/.middleman` directory you can just pull the repository periodically to stay up to date!

```
cd ~/.middleman/hamlman;
git pull
```

## Customizations

### Images

- `images` directory emptied

### JavaScript

- JavaScript manifest is renamed `application.js`
- `javascript/dependencies` directory added
    + includes a [basic Modernizr build](http://modernizr.com/download/#-shiv-cssclasses-load)

### Layouts

- Default layout cleaned up
- `html` element includes `.no-js` class for Modernizr
- Modern `meta` elements added
- `Modernizr` and Stylesheet manifest loaded in head
- JavaScript manifest loaded at the bottom of the document.

### Stylesheets

- Stylesheet manifest is renamed `application.css.scss`
- `stylesheets/dependencies` directory added
    + includes [normalize.css](http://necolas.github.io/normalize.css/)

### Gemfile

- `sass`, `scss-lint`, `middleman-autoprefixer`, and `ejs` added

### Config.rb

- Build options
    + Enables `autoprefixer`
    + Ensures that only `application.css`, `application.js`, and `modernizr.js` are built
    + Minifies all Stylesheets and JavaScript
    + Sets assets and links to relative

### Other Files

- `.editorconfig` added
- `.jshintrc` added
- `.scss-lint.yml` added
