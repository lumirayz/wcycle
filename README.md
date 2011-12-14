Description
-----------
A little script that assigns a randomly selected wallpaper from a directory every DELAY seconds.

Usage
-----
To cycle between all images in ~/wallpapers every minute (60 seconds):
	./wcycle.py -p ~/wallpapers/ -d 60

Notes
-----
* The first wallpaper change is not at program start, but after DELAY seconds.
* This uses nitrogen with --set-zoom-fill, which may not be what you want. You can pretty easily change this in the source code, though.

Compatibility
-------------
Tested on Python 3, but I don't see any problems with Python 2 support, so that might work, too.

License
-------
MIT licensed.
