Heroku buildpack: libspotify
============================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) that vendors libspotify 12.1.51

It is meant to be used in conjunction with other buildpacks as part of a
[multi-buildpack](https://github.com/ddollar/heroku-buildpack-multi).

Usage
-----

Example usage:

    $ heroku config:add BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi.git

    $ cat .buildpacks
    https://github.com/bolster/heroku-libspotify-buildpack.git#1.0
    https://github.com/heroku/heroku-buildpack-python.git#v29


Don't forget to pin buildpack versions you want to use in your .buildpacks file.
