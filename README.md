# Worship songbook (using songs LaTeX package, russian version)

## What?

The purpose of this project is to assemble all known worship songs with their chords in TeX.

As it known simple and truly free way to work with song's lyrics and chords dont exist, but we have TeX and additional songs module - tools to have high-quality result.

Also (my thought): information + system = accessibility.

## Start

On Debian operation system everything you need to work with songs collection is TeX and songs module. Install them with apt-get:

`apt-get install texlive texlive-music`

Then you can just run inside your project folder:

`xelatex songs.tex`

Also, you may be need songidx to make table of contents. Download it from here: http://www.ctan.org/tex-archive/macros/latex/contrib/songs and run `make` inside songidx folder. After that you need to run:

`xelatex songs.tex`

`./songidx.run songsindex.sxd`

And again with index (be cause index pushing page numbering forward):

`xelatex songs.tex`

`./songidx.run songsindex.sxd`

`xelatex songs.tex`

## Links

http://songs.sourceforge.net
