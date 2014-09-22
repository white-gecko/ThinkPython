# Think Python

This repository is a clone/fork of the original [Think Python](http://thinkpython.com) book in Version 2.0.13 as taken from the published [ZIP-File](http://www.greenteapress.com/thinkpython/thinkpython.tex.zip).
I've forked the original code base to fix the ePub creation in its Makefile.

## Usage

Prerequirements: in order to generate the ePub file you have to have the following commands installed (some of them are standart Linux tools the other tools are bundled with calibre):

    latex sed grep pdftops hevea imagen hacha ebook-convert

In order to create an ePub from this repositry is should be as easy as running `make epub`.
But the make instructions require all figures to be available as EPS.
So the full instructions are:

    for f in figs/*.pdf; do pdftops -eps $f; done
    make epub

## License

[Think Python](http://www.greenteapress.com/thinkpython/thinkpython.html) is a Free Book originally written by Allen Downey. It is available under the [Creative Commons Attribution-NonCommercial 3.0 Unported License](http://creativecommons.org/licenses/by-nc/3.0/), which means that you are free to copy, distribute, and modify it, as long as you attribute the work and don't use it for commercial purposes.

The icon files for `up.png`, `back.png` and `next.png` are taken from the [Numix Icon Theme](https://github.com/numixproject/numix-icon-theme-circle) which is licensed under the terms of the GPL-3.0+.
