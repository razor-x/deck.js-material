# Sass Package Skeleton

<!--
[![Bower Version](https://img.shields.io/bower/v/sass-package.svg)](http://bower.io/search/?q=sass-package)
-->
[![MIT License](https://img.shields.io/badge/license-MIT-red.svg)](./LICENSE.txt)
[![Dependency Status](https://img.shields.io/gemnasium/razor-x/sass-package.svg)](https://gemnasium.com/razor-x/sass-package)
[![Build Status](https://img.shields.io/travis/razor-x/sass-package.svg)](https://travis-ci.org/razor-x/sass-package)

Use this project freely as a base for your Sass packages.

## Description

### Features

* [Bower] package structure.
* [Rake] tasks for development.
* Gem management with [Bundler].
* [Travis CI] ready.
* [EditorConfig].
* Badges from [Shields.io]!

[Bundler]: http://bundler.io/
[EditorConfig]: http://editorconfig.org/
[Rake]: https://github.com/jimweirich/rake
[Shields.io]: http://shields.io/
[Travis CI]: https://travis-ci.org/

### Usage

This software can be used freely, see [The Unlicense].
The MIT License text appearing in this software is for
demonstration purposes only and does not apply to this software.

1. Clone this repository or download a [release][Releases].

2. Customize this README.
   - Set the title and summary text.
   - Replace the Description section.
   - Update the Source section.
   - Update the Contributing section.
   - Remove or update the badges.

3. Set the copyright year and owner in `LICENSE.txt`.

4. Customize `bower.json`.

5. Replace any remaining instances of the placeholder package name.
   You can replace the placeholder package name with your own using

````bash
$ git ls-files -z | xargs -0 sed -i 's/sass-package/your-package/g'
$ git ls-files -z | xargs -0 sed -i 's/razor-x/your_username/g'
````

Note that `CHANGELOG.md` is just a template for this skeleton.
The actual changes for this project are documented in the commit history
and summarized under [Releases].

[Releases]: https://github.com/razor-x/sass-package/releases
[The Unlicense]: http://unlicense.org/UNLICENSE

#### Add future update support

If you want to merge in future updates from this skeleton and have your own origin,
set up a separate branch to track this.

````bash
$ git remote rename origin upstream
$ git branch sass-package
$ git branch -u upstream/master sass-package
````

Then add an origin and push master

````bash
$ git remote add origin git@github.com:your_username/your-package.git
$ git push -u origin master
````

Now, the `sass-package` branch will pull changes from this project,
which you can then merge into your other branches.

If you later clone your repo you will need to create the update branch again.

````bash
$ git remote add upstream https://github.com/razor-x/sass-package.git
$ git fetch upstream
$ git checkout -b sass-package upstream/master
````

## Installation

The recommended method is to add this as a dependency
to your project using [Bower] with

````bash
$ bower install --save sass-package
````

Alternatively, you can download a [release][Releases]
or clone the repository directly.

[Bower]: http://bower.io/

## Development and Testing

### Source Code

The [sass-package](https://github.com/razor-x/sass-package)
source is hosted on GitHub.
To clone the project run

````bash
$ git clone https://github.com/razor-x/sass-package.git
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

1. Fork it (https://github.com/razor-x/sass-package/fork).
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
