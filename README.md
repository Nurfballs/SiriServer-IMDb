nurf-IMDb.py
============

Description
-----------
This plugin will allow you to use Siri in conjunction with SiriServer, to query IMBb for information relating to movies / TV shows


Pre-requisites
--------------
1. A working installation of SiriServer.
2. IMDbPy

*The installation and configuraiton of the SiriServer is outside the scope of this readme.*


Installation
------------
1. Download `nurf-imdb.py` and place it in your `/plugins` directory.
2. Edit your `plugins.conf` and add `nurf-imdb` to the list of plugins to load.
3. Install IMDbPy with the following command: `sudo apt-get install python-imdbpy`
4. Restart your SiriServer


Functions
---------

This script supports the following functions

* Get information about a movie
* Lookup director of a movie
* Lookup actor by role (works for TV shows too!)


**Get information about a movie**

Listen String: `(movie lookup)* ([\w ]+)`

Example: say `Movie lookup The Matrix` etc.

[Screenshot](http://i.imgur.com/56tcal.png "Screenshot")

**Lookup director of a movie**

Listen String: `(who directed)* ([\w ]+)`

Example: say `Who directed The Matrix` etc

[Screenshot](http://i.imgur.com/OPlX7l.png "Screenshot")

**Lookup actor by role**

Listen String: `(who played|who plays|who was)* ([\w ]+) *in* ([\w ]+)`

Example: say `Who played Morpheus in The Matrix` etc.

[Screenshot](http://i.imgur.com/XrNqLl.png "Screenshot")


Version History
----------------

**0.1**

* Initial Release