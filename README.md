# handoutWithNotes.sty 2022/02/22 v1.3

Create Handouts with notes from your LaTeX beamer presentation.

–––––––––––––––––––––––––––––––––––––––––––––

Copyright (C) 2009–2018 by Guido Diepen <guido@guidodiepen.nl>
 
Parts provided by Edson Valle

Copyright (C) 2021–2022 Marei Peischl <marei@peitex.de>

***************************************************************************

 This material is subject to the LaTeX Project Public License version 1.3c
 or later. See http://www.latex-project.org/lppl.txt for details.

*************************************************************************

## Quickstart
To use this package load it in a document using beamer and select a layout:

Minimal example:
```
\documentclass{beamer}
\usepackage{handoutWithNotes}
\pgfpagesuselayout{3 on 1 with notes}
\begin{document}
…
\end{document}
```

Currently the following layouts are implemented by this package:

- `1 on 1 with notes landscape`
- `2 on 1 with notes landscape`
- `1 on 1 with notes`
- `2 on 1 with notes`
- `3 on 1 with notes`
- `4 on 1 with notes`

Additionally we support the following package options:

- `slide-frame=true/false` draw a frame around the slides
- `note-frame=true/false` draw a frame around the note pages
- `beamer-notes=true/false` use beamer notepages instead of the area for handwritten notes
- `lines=<Number>` modify the number of lines in the notesbox (default is 8)

Additionally the pgfpages options can be used. for more detailed information use the pdf documentation.

## Version History
* v1.3 (2022-02-22) Clear leftover boxes with notes
* v1.2 (2022-02-02) Add support for DVI–PS–PDF workflows
* v1.1 (2021-11-07)
	- convert the sources for l3build including simple tests
	- add support for graph ruled paper
	- add pdf documentation
* v1.0 (2021-10-21) First CTAN Version
	- add options to draw frames around the slides/notes
	- add possibility to use beamer's note pages instead of empty ones
* 20180920 - Refactored to work with different slide sizes
* 20091202 - Added `1 on 1 with notes` layout, provided by Harald Welte
* 20091108 - Added `2 on 1 with notes landscape` layout, provided by Edson Valle
* 20091104 - Added `3 on 1 with notes` layout
* 20091104 - Added `2 on 1 with notes` layout
* 20091104 - Added `1 on 1 with notes landscape` layout, provided by Edson Valle
* 20090101 - Initial Version