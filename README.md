A web site for sharing literacy materials, especially templates for translation into minority languages.

***

## Quick Start

Make sure you have [Nodejs](http://nodejs.org/download/) and then:

```sh
git clone  https://github.com/BloomBooks/BloomLibrary.git
cd BloomLibrary
sudo npm -g install grunt-cli karma bower  (on Linux)
sudo npm install                           (on Linux)
npm -g install grunt-cli karma bower     (on Windows)
npm install                              (on Windows)
bower install
grunt watch
```

You will need to develop using a local web server (see [Setting Up Your Development Environment -> Server](https://github.com/BloomBooks/BloomLibrary/wiki/Setting-Up-your-Development-Environment#server)).

After pulling new releases, you may need to update various libraries. Do that with


```sh
npm update
bower update
```

## About the grunt files

We built these using [ngBoilerplate](https://github.com/ngbp/ngbp). Read the build.config.js file to see most of what is going on. See the readme of ngBoilerplate for more information. Here are key things:

Grunt merges many vendor and app-specific less files together into the bloom_xyz.css file. The list of these files is main.less.
If you have a css file to load separately, list that in build.config.js.

Normally we have tests run via the offscreen browser phantomjs. If you want to debug using a normal browser, you'll find that setting in karma/X:\dev\BloomLibrary\karma\karma-unit.tpl.js.


## Roadmap

see https://trello.com/b/eO6j48sf/bloom-library

### Contributing

Books may be contributed to the [website](http://www.bloomlibrary.org). Code contributions are welcome also.
We recommend interacting through the Trello board to be sure we're on the same track.

### Search Engine Optimization

A problem with the current approach is that Google and other web crawlers
don't see anything more than our home page. This is discussed at length
at https://docs.google.com/document/d/1XAJRmQoJHYkwkf4CVW_OWiBkRT1jqufKF2rJajcnxIw/edit?usp=sharing.

Copyright and License
=======
Copyright 2013-2016 [SIL International](http://sil.org)
[MIT/X11](http://sil.mit-license.org/)


