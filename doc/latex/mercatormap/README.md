# The LaTeX package mercatormap - version 1.2.0 (2024/08/05)


> Copyright (c) 2020-2024 by Prof. Dr. Dr. Thomas F. Sturm <thomas dot sturm at unibw dot de>

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

- `README.md`                this file
- `CHANGES.md`               log of changes (history)
- `mercatormap.sty`          LaTeX package file (style file)
- `mercatorsupplier.def`     LaTeX package file (include file for style)
- `mercatorpy.def`           LaTeX package file (Python generator)
- `mercatormap.pdf`          Documentation
- `mercatormap.tex`          Source code of the documentation (main file)
- `*.doc.*`                  Source code of the documentation (include files)
- `mercatormap-example.tex`  Source code of an example
- `mercatormap.bib`          Bibliography of the documentation


## Installation

Copy the contents of the `mercatormap.tds.zip` from CTAN to your local TeX file tree.

Alternatively, put the files to their respective locations within the TeX installation:
- `mercatormap.sty`       ->  /tex/latex/mercatormap
- `mercatorpy.def`        ->  /tex/latex/mercatormap
- `mercatorsupplier.def`  ->  /tex/latex/mercatormap
- all other files         ->  /doc/latex/mercatormap
