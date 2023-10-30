# interactive-logic-course
> a interactive course for teaching students logic

Author: Bob Atkey ([GitHub](https://github.com/bobatkey))

## How to build:

Note, you need the following dependencies:
* opam (OCaml package manager)
* make


**Linux** (bash/zsh):

This will first create a local installation of Ocaml in this project, then install all the project dependencies, then ``make`` will translate all the pages from Markdown to HTML, build the ``frontend.js`` file that implements all the interactive bits and copy the fixed assets (CSS, PDFs etc) in to a directory called ``_site`` which will be a local copy of the notes.

1. ``opam switch create . 5.1.0``
2. ``opam intall . --deps-only``
3. ``make``



## Developement

Libaries used: 
* [Ulmus](https://github.com/bobatkey/ulmus)


## Goals
* Implement [CodeMirror](https://codemirror.net/) as a replacement for the code editors
* Write a new lexer parser for CodeMirror to support the custom logic language

