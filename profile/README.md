Zed
===
This is a continuation of the zed project started in 2013 by Zef Hemmel. The scope of this project is to continue the mission of the original authors to build the ultimate simple yet highly efficient code editor.

Welcome to Zed, a code editor built using web technologies, designed to rethink some of the assumptions that underly most editors today. Some of the editor's core features are the features it does not have:

* Tabs
* Always visible file tree
* Menus and buttons and bells and whistles

What you get instead is a bare bones, simple yet powerful editor that focuses on what matters most: making you as productive at editing code and text as possible. To enable this, Zed has:

* Multiple cursors. Once mastered, you will never edit code the same way again.
* Code completion based on symbols defined in your project, current file and snippets.
* Efficient project navigation at various levels of granularity:
* Files, quickly jump to the file you want
* Symbols, Zed indexes all symbols defined in your project and lets you quickly jump to the one you're interested in
* (Vertical) split views, either 1, 2 or 3 vertical splits.
* Auto-updating preview split for various languages (including markdown and coffeescript).
* Editing of local files (via Chrome-specific APIs) and remote files (check the manual on how to do this)

Installation (Chrome App)
=========================

You can install Zed via the Chrome Web Store, or by cloning the github repo:

    $ git clone https://github.com/zedapp/zed.git
    $ cd zed
    $ git submodule update --init

Then, in (a recent version of) Chrome, go to the "three-lined" menu > Tools > Extensions and click the "Load unpacked extension..." button, navigate to the app directory inside the Zed repository checkout. Zed should now run!

Installation (Standalone)
========================

**To build locally:**

    $ git clone https://github.com/zedapp/zed.git
    $ cd zed
    $ git submodule update --init

After this you can either build the version for your platform of choice:

    $ make apps-mac
    $ make apps-win
    $ make apps-linux32

or

    $ make apps-linux64

The builds end up in nw/build and the gzipped versions in release.
Inspiration

Inspiration for Zed comes from:

* Notational Velocity: the goto bar combining search with new file creation
* Apple's iOS and recent Mac file management: abstraction from whether a file is open and by removing the idea that a file has to be explicitly saved.

Contributing
============

If you wish to contribute to this project, start by selecting an open issue and leave a comment suggesting you are going to work on it. Then fork the repo and go ahead and fix ther issue. Then open a pull request where you are going to specify the issue number. We will review and approve/decline/comment on your pr.
Technology

* The excellent ACE editor
* Architect
* jQuery
* Underscore.js
* Require.js

Support
=======

Support via gitip
