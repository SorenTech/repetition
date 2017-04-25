# repetition

*"Repetition and recollection are the same movement, except in oppositie directions, for what is recollected has been, is repeated backward, whereas genuine repetition is crollected forward." - Soren Kierkegaard, Repetition*

## Project Goals

This project aims to radically simplify front-end web development for multiple supported platforms. It does this by providing a platform agnostic file structure, a WebPack configuraton and accompanying NPM scripts, and the option to create routing layers for supported platforms automatically. It is intended to be used alongside gibraltar, our platform agnostic front-end framework. Gibraltar consists of a vuejs single page app which expects to retrieve data over a REST API. It provides generic routing within the app which can be easily translated to the specific routes of a given back-end framework. Repetition provides the tools to complete that routing. It will eventually support the following backends:

 - WordPress (through the REST API)
 - Ghost 
 - Joomla (through a REST API)
 - Drupal (in "headless mode")
 - Squarespace (through the REST API)
 - Contentful
 - Keystone JS
 - Directus
 - Prismic.io
 - others?

## Useage

Basic command structure:

'repetition <backend> (--new)'

The '--new' flag will install the basic source code from gibraltar into 'src' to give you a starting point. This is optional: if you already have a theme or are using a framework other than gibraltar, it can be ommitted.

Repetition will install routing rules based on the specified backend. You can also specify the backend as 'none' or 'all'. 'none' will skip the installation of a routing layer, leaving you with a generic WebPack config and NPM scripts that can be used for any front-end project. 'all' will instruct repeititon to create separate 'dist' folders for every supported backend, allowying you to easily replicate your front-end theme or template across multiple platforms.

## Contributing

Feel free to fork and send pull requests to contribue. You may also report bugs through the GitHub issues tracker.

Please note that this project is just starting and is not yet production ready. We cannot yet offer production level support.

Also, please note that this project is being developed primarily for internal use. You may adopt it freely for your own use, but note that it may not work for your use case. We cannot offer support for use cases outside of our intended use.
