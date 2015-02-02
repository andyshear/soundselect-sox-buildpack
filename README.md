Heroku buildpack: sox
=======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for using [sox](http://sox.sourceforge.net/) in your project.

Lineage
-------

Shamelessly forked from the [ffmpeg heroku buildpack](https://github.com/shunjikonishi/heroku-buildpack-ffmpeg) by [Shunji Konishi](https://github.com/shunjikonishi).

Usage
-----
To use this buildpack, you should prepare a .buildpacks file that contains this buildpack url and your real buildpack url:

    $ ls
    .buildpacks
    
    $ cat .buildpacks
    https://github.com/RBNA/soundselect-sox-buildpack

You can verify that sox is installed by calling:

    $ heroku run "sox"
