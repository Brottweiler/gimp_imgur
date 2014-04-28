A very simple gimp plugin to upload the current image anonymously to imgur.

I created this because I was tired of the seemingly needless steps of exporting the image, and then finding it again in a file browser, when all I really wanted to do was share what I was working on quickly.

Information
-----
There are two kinds of scripts. `imgur-upload.py` and `imgur-flatten-upload.py` will open the link in your favourite web browser, while `imgur-upload-clipboard.py` and `imgur-flatten-upload-clipboard` will copy the link to your clipboard instead.

Requirements
-------
- [GNU Image Manipulation Program](http://gimp.org/)
- [pyperclip](http://coffeeghost.net/2010/10/09/pyperclip-a-cross-platform-clipboard-module-for-python/) (*clipboard* scripts only!)

Install
-------

1. Download the scripts and copy them to your GIMP plug-in directoy.
2. Make sure that the files are executable.

**NOTE** Step 3 is only necessary if you choose to use the *clipboard* scripts!

3. Download [pyperclip.py](http://coffeeghost.net/src/pyperclip.py) and place `pyperclip.py` under `<GIMP install dir>\Python\Lib\pyperclip.py` on Windows, and under `/usr/lib/gimp/2.0/python/pyperclip.py` on GNU/Linux.


Usage
-----
Entries will be added to the filter menu under the Imgur heading. Both will create a temporary file in your systems temporary directory and then upload that .png directly to imgur. Depending on what script you use (you can use all of them) it will either open the link in your favourite web browser, or copy the link to your clipboard.

There is no support for deleting the image currently.

Note that the flatten and upload will flatten your image as part of the upload, however this will register as a normal operation and can be undone safely.
