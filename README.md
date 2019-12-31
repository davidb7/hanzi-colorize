.. image:: https://circleci.com/gh/cayennes/kanji-colorize.svg?style=svg
    :target: https://circleci.com/gh/cayennes/kanji-colorize

==============
HanziColorizer
==============

.. image:: kanji-colorize-examples.png

About
-----

``kanji_colorize.py`` is a script for coloring, resizing, and renaming
the stroke order diagrams from the
`HanziVG <https://github.com/Connum/hanzivg>`_ project.  This is a fork from 
the `KanjiColorizer <https://github.com/cayennes/kanji-colorize>` project and is 
meant to be the Hanzi version for `anki <http://ankisrs.net/>`.

Using with Anki
---------------

There is currently no Anki plugin yet. I will update this section when 
it is ready.

Downloading and Running the Software
------------------------------------

The `kanji_colorize.py` script makes it possible to generate diagrams to your
own specifications.  It may have issues with a python not built with
wide-character support

Development
-----------

Activate the virtual environment and install requirements:

.. code:: bash

    $ python3 -m venv venv
    $ source venv/bin/activate
    $ pip install -r requirements.txt

To run the existing tests:

.. code:: bash

    $ python -m kanjicolorizer.colorizer
    $ python -m unittest discover -s kanjicolorizer

To create a new release:

.. code :: bash

    $ paver dist_anki_addon

Test by unzipping the zip file in `dist` into a new directory in `~/.local/share/Anki2/addons21` (or the equivalent for the OS being tested).

License
-------

The code is available under the Affero GPL version 3 or later and the SVG
images are available under Creative Commons Attribution-Share Alike 3.0.
See file headers and files in ``licenses/`` for more information.
