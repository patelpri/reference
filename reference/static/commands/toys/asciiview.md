asciiview
-------
aview and asciiview are image views that show images in ASCII art.

aview will convert a .pnm image into an ascii art format. It supports zooming, unzooming, inversion, contrast, brightness and gamma control. It also allows you to save to many formats.

asciiview converts the file formats into PNM using ImageMagin or NetPBM and start aview.
Therefore, asciiview accepts files that are not in the PNM format, while aview cannot.

### Syntax

A few examples of aview and asciiview commands to run:
~~~ bash
asciiview [options] filename.jpg
~~~
or
~~~ bash
aview [options] filename.p[ngbp]m
~~~
---

### Options

All options can be found using:

~~~ bash
aview --help
~~~

Here are a few options to further customize your images with aview or asciiview. As a note, these options will with both asciiview and aview.

~~~ bash
-width		set width
-height		set hight
-inverse	enables the inverse rendering of image
-contrast <val> set contrast (0-255)
-bright <val> 	set brightness (0-255)
-boldfont	enable boldfont
-extended	uses all 256 characters
~~~

### Examples

~~~ bash
aview cat.pnm
~~~~

~~~ bash
asciiview earth_and_moon.jpg
~~~

The examples above will simply show your cat and earth_and_moon images in ASCII art.

~~~ bash
asciiview -inverse earth_and_moon.jpg

aview -contrast 255 cat.pnm
~~~

The examples above show how you can add options in front of the filename to customize these images as you please. 
The inverse command will inverse the rendering of the image. The contrast command will set the contrast from 0 to 100% depending on the entered value (0-255).
