# [sanjibsen/texlive-thin](http://hub.docker.com/r/sanjibsen/texlive-thin/)

[![Docker Pulls](http://img.shields.io/docker/pulls/sanjibsen/texlive-thin.svg)](http://hub.docker.com/r/sanjibsen/texlive-thin/)
[![Docker Stars](http://img.shields.io/docker/stars/sanjibsen/texlive-thin.svg)](http://hub.docker.com/r/sanjibsen/texlive-thin/)

This is a Docker image containing a [`TeX Live`](http://en.wikipedia.org/wiki/TeX_Live) installation with several fonts.
It is an alternative to my significantly bigger, full `Tex Live` installation in docker, namely [texlive-full](http://www.github.com/sanjib-sen/texlive-full).
While the name of this image includes `thin`, it is not a minimal `Tex Live` installation.
It does contain some additional and basic packages (e.g. curl, git) as well as fonts, but nothing as funky as in the other container.

## 1. Building and Components

The image has the following components:

- [`TeX Live`](http://www.tug.org/texlive/)
- ~~[`ghostscript`](http://ghostscript.com/)~~ (Can be added by uncommenting the package name in the Dockerfile)
- ~~[`poppler-utils`](http://poppler.freedesktop.org/)~~ (Can be added by uncommenting the package name in the Dockerfile)

## 2. License

This image is licensed under the GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007, which you can find in file [LICENSE.md](http://github.com/thomasWeise/docker-texlive/blob/master/LICENSE.md).
The license applies to the way the image is built, while the software components inside the image are under the respective licenses chosen by their respective copyright holders.

<!-- ### 3. Utility Scripts

Currently, we provide the following utility scripts in folder `/bin/`:

- `filterPdf.sh <document>` transform a document (either in [PostScript](http://en.wikipedia.org/wiki/PostScript)/`PS`, `EPS`, or `PDF` format) to `PDF` and include as many of the fonts used inside the document into the final `PDF`. This uses ghostscripts `gs` and checks the output with `pdftotext` from `poppler-utils` before replacing `<document>` with the hope to build a final pdf that can display on as many machines correctly as possible. -->

## 4. Contact

If you have any questions or suggestions, please contact [Sanjib Kumar Sen](mailto:sksenonline@gmail.com)
