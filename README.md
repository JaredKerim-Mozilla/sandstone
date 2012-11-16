Sandstone
=========

A bootstrap for sites in the Mozilla Universe. This project aims to automate as much
of the process of starting a new website using the Mozilla Sandstone theme as possible and,
also provides the tools, via Grunt, to preprocess, lint and minify/uglify the assets.

*NOTE:* For sites based on Django/Playdoh, the Grunt file is not currently included.

Prerequisites
=============

You will currently need to follow prerequisites installed:

* [Nodejs][nodejs]
* [LESS][less]
* [Grunt][grunt]

To intall the LESS preprocessor run the following after installing Nodejs

    (sudo) npm install -g less

Next install Grunt:

    (sudo) npm install -g grunt

You may be required to use sudo but, in most cases it will be optional.

Usage
=====

Inside the directory you wish to create your project clone Sandstone:

    git clone git@github.com:ossreleasefeed/Sandstone.git yourprojectname

Once completed, change directory into your project folder and run:

    npm install

This will install any additional dependencies defined inside package.json. Inside your new project folder
there will also be a .gitignore file that will ensure that the node_modules folder created above, as well
as any .css files will not be included in source control.

Feel free to add any additional exclusions you require.

Grunt Tasks
===========

The current [Grunt][grunt] tasks included:

    grunt

This will run the default task which uses lessc to preprocess your .less files

    grunt lint

This will lint, using JSHint, your grunt file itself as well as all .js files inside the
js folder.

[nodejs]: http://nodejs.org
[less]: https://github.com/cloudhead/less.js
[grunt]: http://github.com/cowboy/grunt
