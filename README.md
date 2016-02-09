# AVHershey-OTF

**NB: This is a preliminary release, and each font file does not
  contain enough character glyphs for useful typesetting. As is, this
  distribution is _not yet_ recommended for the general user.**

A simple conversion of some subsets of the
“[Hershey fonts](https://en.wikipedia.org/wiki/Hershey_fonts)” to
OpenType format. All curves are approximated with short straight line segments.

## Files

1. *otf/* - OpenType font binaries for three subsets — Simplex (single
   line, sans-serif), Duplex (outline, sans-serif) and Complex
   (multi-line, serif) — in three weights: Light, Medium and Heavy,
   roughly corresponding to plotter renderings with a thin, medium or
   thick pen.

2. *sfd/* - [FontForge](https://fontforge.github.io/ "FontForge")
   source files.


## Workflow

Building from my previous
[python-hershey](https://github.com/scruss/python-hershey
"python-hershey") project, the Hershey font vectors were converted to
buffered polygons using
[Shapely](http://toblerity.org/shapely/project.html). These polygons
were saved as SVG, and (along with the character glyph kerning
information) were imported into FontForge.

## Acknowledgements

* Derived from character stroke coordinates by Allen V. Hershey
  published in "Calligraphy for Computers" (US Naval Weapons
  Laboratory, 1967-08-01, NWL Report No. 2101, NTIS accession number
  AD-662 398) and elsewhere. These coordinates were published without
  copyright.

* The efforts of the Usenet Font Consortium (James Hurt, et al) who
  reformatted Hershey's data and published it to mod.sources on
  1986-04-01 [Volume 4, Issue 42] are greatly appreciated.

## Todos

1. Extract more font styles from the Hershey coordinate tables.

2. Fill in/create basic characters to complete ASCII set.

3. Add basic accented characters.

## Author

Stewart C. Russell - http://scruss.com/blog/

## Licence

Dual-licensed CC0/WTFPL. (Srsly; see COPYING.)
