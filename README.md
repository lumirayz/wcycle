Description
-----------
A little script that assigns a randomly selected wallpaper from a directory every DELAY seconds.

Usage
-----
To cycle between all images in ~/wallpapers every minute (60 seconds):

	./wcycle.py -p ~/wallpapers/ -d 60

Notes
-----
* The first wallpaper change is not at program start, but after DELAY seconds, you can toggle this with the `--instant` option.
* This uses nitrogen with --set-zoom-fill by default, which may not be what you want. You can use the `--command` option to customize this.

Compatibility
-------------
Tested on Python 3, but I don't see any problems with Python 2 support, so that might work, too.

Usage
-----

	Usage: wcycle [options]
	
	Options:
	  -h, --help            show this help message and exit
	  -p PATH, --path=PATH  path to get images from
	  -d DELAY, --delay=DELAY
		                    delay between image switches
	  -e EXTENSIONS, --extensions=EXTENSIONS
		                    comma separated list of allowed extensions
	  -c COMMAND, --command=COMMAND
		                    command to execute on wallpaper change, replaces %f
		                    with the path to the wallpaper
	  -i, --instant         don't wait before first wallpaper change

License
-------
MIT licensed.
