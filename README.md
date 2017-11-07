# Usage
There are two ways to use the .sty files
## simple
Just put them in your current project directory (i.e. where the main .tex file resides)
and include either with `\usepackage{standardsetup}` or `\usepackage{beamersetup}`.
Note that `beamersetup` loads `standardsetup` internally, so only load one.

## user installation
- set `export TEXMFHOME=${HOME}/.texfm/` (or to any path you prefer)
- create the directory path `${TEXMFHOME}/tex/latex`
- link the `Resource` directory into the new `latex` directory
Now tex should find both packages. (Make sure it was run from a shell where `TEXMFHOME` is
properly set.)
