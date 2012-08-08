resources-go
============

An assets-loading package for Go.

Applications can use this package to load assets from zip-files (incuding a zip file bundled in the executable),
the filesystem, or other sources through a single interface. Also allows for the building of a search path to access
files sequentially through a set of application defined locations.

Installation
------------

go get github.com/cookieo9/resources-go/v1/resources

Embedding Zip-Files
-------------------

To embed a zip file into your executable do the following:
 - Create executable (eg: go build -o myApp)
 - Create zip file  (eg: zip -r assets.zip assets)
 - Append zip file to executable (eg: cat assets.zip >> myApp)
 - Adjust the offsets in the zip header [optional] (zip -A myApp)

License
-------
http://cookieo9.mit-license.org/2012