HexGL
=========

Source code of [HexGL](http://hexgl.bkcore.com), the futuristic HTML5 racing game by [Thibaut Despoulain](http://bkcore.com)

## License

Unless specified in the file, HexGL's code and resources are licensed under the *Creative Commons Attribution-NonCommercial 3.0 Unported License*.

To view a copy of this license, visit http://creativecommons.org/licenses/by-nc/3.0/.

If you feel like you deserve another license for a special case, [drop me a note](http://bkcore.com/contact.html), and we'll talk about it.

## Installation

	cd ~/
	git clone git://github.com/BKcore/HexGL.git
	cd HexGL
	python -m SimpleHTTPServer
	chromium index.html

## Regarding the code

As of now the code is pretty much raw and undocumented. I'll be commenting it someday, but that won't be until I've finished the next content update and code refactoring sorry!
There will also be some refactoring, when I get some time :P

## Note

After much thinking, I've decided to release HexGL's source code under CC 3.0 BY-NC until further notice. This is not a definite choice, and the game may end up under the MIT license someday.

Feel free to post issues, patch or anything to make the game better.

## Package with Crosswalk Runtime
1. Download Crosswalk Runtime from https://download.01.org/crosswalk/releases/crosswalk/android/stable/6.35.131.13/crosswalk-6.35.131.13.zip
2. Unzip the downloaded zip, and run the command:

  python make_apk.py --name=HexGLDemo --icon=/path/to/HexGL/icon_64.png --package=org.xwalk.hexgldemo --xwalk-command-line=”--ignore-gpu-blacklist” --orientation=landscape --enable-remote-debugging --app-root=/path/to/HexGL --app-local-path=index.html

3. On success, you will HexGLDemo_arm.apk file in the crosswalk directory.
