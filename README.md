A very simple gimp plugin to upload the current image anonymously to imgur.

I created this because I was tired of the seemingly needless steps of exporting the image, and then finding it again in a file browser, when all I really wanted to do was share what I was working on quickly.

Requirements
-------
- [GNU Image Manipulation Program](http://gimp.org/)
- [pyperclip](http://coffeeghost.net/2010/10/09/pyperclip-a-cross-platform-clipboard-module-for-python/)

Install
-------

1. Download [pyperclip.py](http://coffeeghost.net/src/pyperclip.py) and place `pyperclip.py` under `<GIMP install dir>\Python\Lib\pyperclip.py` on Windows, and under `/usr/lib/gimp/2.0/python/pyperclip.py` on GNU/Linux.
2. Download the scripts and copy them to your GIMP plug-in directoy.
3. Make sure that the files are executable.

Usage
-----
Entries will be added to the filter menu under the Imgur heading.  Both will create a temporary file in your systems temporary directory and then upload that .png directly to imgur.  After which the link will be copied to your clipboard.

There is no support for deleting the image currently.

Note that the flatten and upload will flatten your image as part of the upload, however this will register as a normal operation and can be undone safely.
