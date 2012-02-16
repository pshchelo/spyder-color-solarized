================================================
Solarized for Spyder IDE
================================================

About
=====

This is an attempt to include support of the Solarized color scheme
into Spyder Python IDE.

This project repository is found on GitHub at
https://github.com/pshchelo/spyder-color-solarized.

This project is released under MIT license (see LICENSE.txt), as both 
Solarized and Spyder themselves.

About Solarized color scheme, citing its author 
Ethan Schoonover (http://ethanschoonover.com/solarized)\:

	Solarized is a sixteen color palette (eight monotones, eight accent colors) 
	designed for use with terminal and gui applications. 
	It has several unique properties. 
	I designed this colorscheme with both precise CIELAB lightness 
	relationships and a refined set of hues based on fixed color wheel 
	relationships. 
	It has been tested extensively in real world use on color calibrated 
	displays (as well as uncalibrated/intentionally miscalibrated 	displays) 
	and in a variety of lighting conditions.

The main repository of Solarized Color Scheme is found on GitHub at
https://github.com/altercation/solarized.

About Spyder (http://code.google.com/p/spyderlib):

	Spyder (previously known as Pydee) is a powerful interactive development 
	environment for the Python language with advanced editing, interactive 
	testing, debugging and introspection features.


Installation Instructions
=========================

I have not yet found a way to include Solarized support as a Spyder plugin,
so the solution I use is to meddle with configuration files.

#. Close all instances of Spyder if it is running.
#. Find a Spyder config file at ``~/.spyder2/.spyder.ini`` on \*nix/BSD/MacOSX 
   or ``c:\Users\[yourusername]\.spyder2\.spyder.ini`` on Windows Vista/7.
   You may have to turn the display of hidden files on to find this folder 
   and this file. Open this file with the text editor of your choice.
#. Find a section named ``[color_schemes]`` inside this file.
#. Replace the next line (starting with ``names =`` ...) with the content
   of the ``spyder.ini`` file in this repo (note that I intentionally omitted 
   the leading dot in the included file name so that it is not hidden).
#. Save and close ``.spyder.ini``, start Spyder and choose SolLight or SolDark as your 
   editor color scheme in ``Preferences -> Editor -> Display -> Syntax color scheme``.
   

Screenshots
===========

.. image:: https://github.com/pshchelo/spyder-color-solarized/raw/master/spyder-SolLight.png
   :width: 400px
   :alt: Spyder with Solarized Light
   :target: https://github.com/pshchelo/spyder-color-solarized/raw/master/spyder-SolLight.png
.. image:: https://github.com/pshchelo/spyder-color-solarized/raw/master/spyder-SolDark.png
   :width: 400px
   :alt: Spyder with Solarized Dark
   :target: https://github.com/pshchelo/spyder-color-solarized/raw/master/spyder-SolDark.png


Contributing
============
This work is in progress, and although some color assignments 
(text, background, comments, side area/current line) are pretty 
much set solid by following the principles of the original Solarized scheme, 
improvement suggestions for the other assignments are very welcome.


Current color assignments
=========================

+------------------+----------------------+----------------+
|                  | Solarized color name | Hex color code |
|  Spyder element  +----------+-----------+--------+-------+
|                  |   Light  |   Dark    |  Light | Dark  |
+==================+==========+===========+========+=======+
| Background       | base3    | base03    |#fdf6e3 |#002b36|
+------------------+----------+-----------+--------+-------+
| Current line     | base2    | base02    |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+
|                  |          |           |        |       |
+------------------+----------+-----------+--------+-------+

Spyder element			Light		LightHex	Dark		DarkHex

Background				base3		#fdf6e3		base03		#002b36
Current line			base2		#eee8d5		base02		#073642 
Occurrence				blue		#268bd2		blue		#268bd2 
Link					base01		#586e75		base1		#93a1a1
Side areas				base2		#eee8d5		base02		#073642 
Matched brackets		blue		#268bd2		blue		#268bd2
Unmatched brackets		red			#dc322f		red			#dc322f
Normal text				base00		#657b83		base0		#839496
Keyword					green		#859900		green		#859900
Built-in				violet		#6c71c4		violet		#6c71c4
Definition				magenta-b	#d33682		magenta-b	#d33682
Comment					base1-i		#93a1a1		base01-i	#586e75
String					cyan		#2aa198		cyan		#2aa198
Number					orange		#cb4b16		orange		#cb4b16
Instance				yellow-i	#b58900		yellow-i	#b58900

