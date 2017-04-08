# Naming standards and conventions

* The following files are provided for your configuration:

    - `config.tex`: The names of you, your committee members, department, and defense year
    - `brege.sty`: Personal commands used in the manuscript
    - `wsudissertation.tex`: WSU dissertation formatting

* The root of the manuscript is in:

    - `00-dissertation.tex`: Comment chapters and bibliography for quick debugging

* All front matter is given in 0?-{*,name-of-section}.tex files.  These are:

    - `01-title.tex`: The title page
    - `02-signatures.tex`: The signature page
    - `03-copyright.tex`: The copyright
    - `04-acknowledgements.tex`: Your acknowledgements
    - `05-abstract.tex`: Your abstract section
    - `06-lists.tex`: Table of contents and list of figures & tables
    - `07-dedication.tex`: You dedication page

* All of the chapters are:

    - `11-chapter-1.tex`: Overview chapter
    - `12-chapter-2.tex`: Equations of State
    - `13-chapter-3.tex`: Numerical Methods
    - `14-chapter-4.tex`: Nuclear EOS's in `SpEC`
    - `15-chapter-5.tex`: Results of Nuclear EOS Survey

* The bibliography shall be in:

    - `21-references.bib`: Uses `BibTeX` entries ([gscholar.py](https://github.com/venthur/gscholar) is your friend)
