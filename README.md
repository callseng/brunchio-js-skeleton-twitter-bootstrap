# Brunch with js
This is a simple js skeleton for [Brunch](http://brunch.io/).  I've
modified it to include Twitter Bootstrap.

Main languages are JavaScript,
[Stylus](http://learnboost.github.com/stylus/), 
[Backbone](http://documentcloud.github.com/backbone/),
[Underscore](http://documentcloud.github.com/underscore/),
[Twitter Bootstrap](http://twitter.github.com/bootstrap/)


## Quick Start
brunch new YOUR_APP_NAME --skeleton git://github.com/briaar/brunchio-js-skeleton-twitter-bootstrap.git

## Getting started with Brunch

Clone the repo and run `npm install` & `brunch build`.
See more info on the [official site](http://brunch.io)

## Overview

    config.coffee
    README.md
    /app/
      /assets/
        index.html
        images/
      /lib/
      models/
      styles/
      views/
        templates/
      application.js
      initialize.js
    /test/
      functional/
      unit/
    /vendor/
      scripts/
        backbone.js
        jquery.js
        console-helper.js
        underscore.js
      styles/
        normalize.css
        helpers.css

* `config.coffee` contains configuration of your app. You can set plugins /
languages that would be used here.
* `app/assets` contains images / static files. Contents of the directory would
be copied to `build/` without change.
Other `app/` directories could contain files that would be compiled. Languages,
that compile to JS (coffeescript, roy etc.) or js files and located in app are 
automatically wrapped in module closure so they can be loaded by 
`require('module/location')`.
* `app/models` & `app/views` contain base classes your app should inherit from.
* `test/` contains feature & unit tests.
* `vendor/` contains all third-party code. The code wouldn’t be wrapped in
modules, it would be loaded instantly instead.

This all will generate `public/` (by default) directory when `brunch build` or `brunch watch` is executed.

## Other
Versions of software the skeleton uses:

* jQuery 1.7.2
* Backbone 0.9.1
* Underscore 1.3.3
* HTML5Boilerplate 3.0.3

The license is [public domain](http://creativecommons.org/publicdomain/zero/1.0/).
Use it however you want.
