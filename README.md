# The LaTeX package mercatormap - version 1.3.1 (2026/06/03)

[![CTAN](https://img.shields.io/ctan/v/mercatormap.svg)](https://www.ctan.org/pkg/mercatormap)

> Copyright (c) 2020-2026 by Prof. Dr. Dr. Thomas F. Sturm <thomas dot sturm at unibw dot de>

> This work may be distributed and/or modified under the
> conditions of the LaTeX Project Public License, either version 1.3
> of this license or (at your option) any later version.
> The latest version of this license is in
>   https://www.latex-project.org/lppl.txt
> and version 1.3c or later is part of all distributions of LaTeX
> version 2008-05-04 or later.

> This work has the LPPL maintenance status `author-maintained`.

> This work consists of all files listed in README.md


The mercatormap package extends TikZ with tools to
create map graphics. The provided coordinate system relies on the
Web Mercator projection used on the Web by OpenStreetMap and others.
The package supports the seamless integration of graphics
from public map tile servers by a Python script. Also, common map
elements like markers, geodetic networks, bar scales, routes, orthodrome
pieces, and more are part of the package.


## Contents of the package

- `README.md`                    this file
- `CHANGELOG.md`                 log of changes (history)
- `tex/mercatormap.sty`          LaTeX package file (style file)
- `tex/mercatorsupplier.def`     LaTeX package file (include file for style)
- `tex/mercatorpy.def`           LaTeX package file (Python generator)
- `doc/mercatormap.pdf`          Documentation
- `doc/mercatormap.tex`          Source code of the documentation (main file)
- `doc/*.doc.*`                  Source code of the documentation (include files)
- `doc/mercatormap-example.tex`  Source code of an example
- `doc/mercatormap.bib`          Bibliography of the documentation


## Installation

Install the files in the appropriate locations within your local TeX file tree.

- `tex/mercatormap.sty`       ->  /tex/latex/mercatormap
- `tex/mercatorpy.def`        ->  /tex/latex/mercatormap
- `tex/mercatorsupplier.def`  ->  /tex/latex/mercatormap
- all other files             ->  /doc/latex/mercatormap
