# deck.js Material Theme

[![Bower Version](https://img.shields.io/bower/v/deck.js-material.svg)](http://bower.io/search/?q=deck.js-material)
[![MIT License](https://img.shields.io/badge/license-MIT-red.svg)](./LICENSE.txt)
[![Dependency Status](https://img.shields.io/gemnasium/razor-x/deck.js-material.svg)](https://gemnasium.com/razor-x/deck.js-material)
[![Build Status](https://img.shields.io/travis/razor-x/deck.js-material.svg)](https://travis-ci.org/razor-x/deck.js-material)

Material theme for deck.js.

## Description

### Requirements

[Bower], [Bourbon], [Neat], and [deck.js].

Additionally, this theme uses the [Roboto] and [Open Sans] fonts,
so you should provide them, e.g., with [Web Font Loader].

Other dependencies are managed via Bower.
Make sure your Bower components directory is in your Sass load path.

[Bourbon]: http://bourbon.io/
[deck.js]: http://imakewebthings.com/deck.js/
[Neat]: http://neat.bourbon.io/
[Open Sans]: https://www.google.com/fonts/specimen/Open+Sans
[Roboto]: https://www.google.com/fonts/specimen/Roboto
[Web Font Loader]: https://developers.google.com/fonts/docs/webfont_loader

### Usage

This theme assumes you have already imported
Bourbon and Neat into your project.
Additionally, you should import the reset theme
included with deck.js.

For example, this will work with most modern build systems,

````sass
@import bourbon
@import neat
@import deck.js/themes/style/reset
@import deck.js-material
````

## Installation

Add this as a dependency
to your project using [Bower] with

````bash
$ bower install --save deck.js-material
````

[Bower]: http://bower.io/

## Development and Testing

### Source Code

The [deck.js-material](https://github.com/razor-x/deck.js-material)
source is hosted on GitHub.
To clone the project run

````bash
$ git clone https://github.com/razor-x/deck.js-material.git
````

### Requirements

You will need [Ruby] ≥ 2 with [Bundler] and [Bower].

Install the development dependencies with

````bash
$ bundle
````

[Ruby]: https://www.ruby-lang.org/

### Rake

Run `rake -T` to see all Rake tasks.

````
rake build  # Compile Sass to CSS
rake clean  # Remove build directory
rake watch  # Have Sass watch for changes
````

## Contributing

Please submit and comment on bug reports and feature requests.

To submit a patch:

1. Fork it (https://github.com/razor-x/deck.js-material/fork).
2. Create your feature branch (`git checkout -b my-new-feature`).
3. Make changes.
4. Commit your changes (`git commit -am 'Add some feature'`).
5. Push to the branch (`git push origin my-new-feature`).
6. Create a new Pull Request.

## License

This Sass package is licensed under the MIT license.

## Warranty

This software is provided "as is" and without any express or
implied warranties, including, without limitation, the implied
warranties of merchantibility and fitness for a particular
purpose.
