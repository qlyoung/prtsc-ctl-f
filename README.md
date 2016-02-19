prtsc-ctl-f
===========
*dump all visible text on your screen*

This is a simple python script that glues together a random screenshot
function I found on StackOverflow with the Tesseract OCR library to
give you an amazingly powerful and innovative tool that takes a screenshot,
runs it through Tesseract, and dumps any recognized text to stdout.

Technically you could do this with

    $ scrot
    $ tesseract -c <configvars> <image>

on any system, but, you know, Python is fun.

Usage
-----

    $ python prtsc-ctl-f.py
    $ python prtsc-ctl-f.py | grep <search term>

Dependencies
------------
Debian:

    # apt-get install tesseract-ocr
    
Fedora/RH:

    # yum install tesseract

License
-------
```
Copyright (C) 2015  Quentin Young

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see http://www.gnu.org/licenses/.
```
