# handoutWithNotes.sty 2021/10/21 v1.0

Create Handouts with notes from your LaTeX beamer presentation.
This package provides pgfpages layouts to place notes next to the scaled slides.
By default the note area is empty providing rules for handwritten notes but with version 1.0 also beamer note pages can be used there.

–––––––––––––––––––––––––––––––––––––––––––––

 Copyright (C) 2009–2018 by Guido Diepen <guido@guidodiepen.nl>
     Parts provided by Edson Valle
 Copyright (C) 2021 Marei Peischl <marei@peitex.de>

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

Additionally the pgfpages options can be used.


## Documentation
A detailed documentation will follow but until this is done most information can be found in the blog post: https://www.guidodiepen.nl/2009/07/creating-latex-beamer-handouts-with-notes/

## Version History
* v1.01 (2021-11-xx)
	- use l3build
	- add support for graph ruled paper
* v1.00 (2021-10-21) First CTAN Version
	- add options to draw frames around the slides/notes
	- add possibility to use beamer's note pages instead of empty ones
* 20180920 - Refactored to work with different slide sizes
* 20091202 - Added `1 on 1 with notes` layout, provided by Harald Welte
* 20091108 - Added `2 on 1 with notes landscape` layout, provided by Edson Valle
* 20091104 - Added `3 on 1 with notes` layout
* 20091104 - Added `2 on 1 with notes` layout
* 20091104 - Added `1 on 1 with notes landscape` layout, provided by Edson Valle
* 20090101 - Initial Version