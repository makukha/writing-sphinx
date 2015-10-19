# Best practices template for writing documentation (with Sphinx)

## Features

1. **Write in plain text** using [reStructuredText](http://docutils.sourceforge.net/rst.html) syntax
    with reach [markup features](http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html) and multiple.
2. **Generate beautiful documents** with highly customizable [Sphinx](http://sphinx-doc.org)
    with multiple [extensions](http://sphinx-doc.org/extensions.html) available.
3. **Get document in various formats**: HTML, PDF (LaTeX), Epub, and many others.
4. **Automate document generation** with [Tox](https://tox.readthedocs.org).

## Installation

- Install [Python 3](https://www.python.org) (may be already installed on your system).
- Install [Tox](https://tox.readthedocs.org): ``pip3 install tox``.
- Install [Git](https://git-scm.com).
- Clone this repository.

## Usage

- Edit project author, title and copyright metadata in **conf.py**.
- Edit source files in starting from root **index.rst**.
- Compile document by running for example ``tox -e singlehtml`` from the repository root directory.
    Allowed targets are all [builders supported by Sphinx](http://sphinx-doc.org/builders.html):
    **singlehtml** (default), **html**, **dirhtml**, **pickle**, **json**,
    **htmlhelp**, **qthelp**, **applehelp**, **devhelp**,
    **epub**, **latex**, **latexpdf**, **latexpdfja**, **text**, **man**, **texinfo**, **info**,
    **gettext**, **changes**, **linkcheck**, **doctest**, **coverage**, **xml**, **pseudoxml**.
- Store image files in **static**.
