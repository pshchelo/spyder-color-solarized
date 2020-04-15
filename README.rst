========================
Solarized for Spyder IDE
========================

Status - archived since 2020-04-15
==================================

I am no longer a Spyder user, so this is effectively abandoned.

Leaving it here for Spyder 2.x and Spyder 3.0 users.

For Spyder 3.1 there is a pull request
https://github.com/spyder-ide/spyder/pull/3534
that proposes it to master and probably will be backported to 3.1 -
please help the author to merge it and enjoy Solarized in
Spyder out-of-the-ox :)

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

About Spyder (https://github.com/spyder-ide/spyder):

	Spyder (previously known as Pydee) is a powerful interactive development
	environment for the Python language with advanced editing, interactive
	testing, debugging and introspection features.


Installation Instructions
=========================

I have not yet found a way to include Solarized support as a Spyder plugin,
so the solution I use is to tinker with configuration files.

#. Close all instances of Spyder if it is running.
#. Find a Spyder config file at ``~/.spyder2/.spyder.ini`` on \*nix/BSD/MacOSX
   or ``c:\Users\[yourusername]\.spyder2\.spyder.ini`` on Windows Vista/7.
   You may have to turn the display of hidden files on to find this folder
   and this file. Open this file with the text editor of your choice.
#. Find a section named ``[color_schemes]`` inside this file.
#. Replace the next line (starting with ``names =`` ...) with the content
   of the ``spyder.ini`` file in this repo (note that I intentionally omitted
   the leading dot in the included file name so that it is not hidden).
#. Save and close ``.spyder.ini``, start Spyder and choose
   SolarizedLight or SolarizedDark as your editor color scheme in
   ``Preferences -> Editor -> Display -> Syntax color scheme``.


Screenshots
===========

.. image:: https://github.com/pshchelo/spyder-color-solarized/raw/master/spyder-SolLight.png
   :width: 100px
   :alt: Spyder with Solarized Light
   :target: https://github.com/pshchelo/spyder-color-solarized/raw/master/spyder-SolLight.png
.. image:: https://github.com/pshchelo/spyder-color-solarized/raw/master/spyder-SolDark.png
   :width: 100px
   :alt: Spyder with Solarized Dark
   :target: https://github.com/pshchelo/spyder-color-solarized/raw/master/spyder-SolDark.png


Current color assignments
=========================

+--------------------+----------------------+-------------------+----------+
|                    | Solarized color name |   Hex color code  |          |
|  Spyder element    +-----------+----------+---------+---------+  Style   +
|                    |   Light   |   Dark   |  Light  |   Dark  |          |
+====================+===========+==========+=========+=========+==========+
| Background         |   base3   |  base03  | #fdf6e3 | #002b36 |          |
+--------------------+-----------+----------+---------+---------+----------+
| Current line       |   base2   |  base02  | #eee8d5 | #073642 |          |
+--------------------+-----------+----------+---------+---------+----------+
| Occurrence         |   base0   |  base00  | #839496 | #657b83 |          |
+--------------------+-----------+----------+---------+---------+----------+
| Link               |        magenta       |      #d33682      |          |
+--------------------+-----------+----------+---------+---------+----------+
| Side areas         |   base2   |  base02  | #eee8d5 | #073642 |          |
+--------------------+-----------+----------+---------+---------+----------+
| Matched brackets   |   base01  |  base1   | #586e75 | #93a1a1 |          |
+--------------------+-----------+----------+---------+---------+----------+
| Unmatched brackets |          red         |      #dc322f      |          |
+--------------------+-----------+----------+---------+---------+----------+
| Normal text        |   base00  |  base0   | #657b83 | #839496 |          |
+--------------------+-----------+----------+---------+---------+----------+
| Keyword            |         green        |      #859900      |          |
+--------------------+-----------+----------+---------+---------+----------+
| Built-in           |         violet       |      #6c71c4      |          |
+--------------------+-----------+----------+---------+---------+----------+
| Definition         |          blue        |      #268bd2      | **bold** |
+--------------------+-----------+----------+---------+---------+----------+
| Comment            |   base1   |  base01  | #93a1a1 | #586e75 | *italic* |
+--------------------+-----------+----------+---------+---------+----------+
| String             |          cyan        |      #2aa198      |          |
+--------------------+-----------+----------+---------+---------+----------+
| Number             |         orange       |      #cb4b16      |          |
+--------------------+-----------+----------+---------+---------+----------+
| Instance           |         yellow       |      #b58900      | *italic* |
+--------------------+-----------+----------+---------+---------+----------+
