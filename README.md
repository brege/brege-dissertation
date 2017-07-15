# Naming standards and conventions

*   The following files are provided for your configuration:

    -   `config.sty`: The names of you, your committee members,
	department, and defense month &amp; year
    -   `brege.sty`: Personal commands used in the manuscript
    -   `wsudissertation.sty`: WSU dissertation formatting

*   The root of the manuscript is in:

    -   `00-dissertation.tex`: Comment chapters and bibliography for 
	quick debugging

*   All front matter is given in `0[1-7]-{*,name-of-section}.tex` files.
    These are:

    -   `01-title.tex`: The title page
    -   `02-copyright.tex`: The copyright
    -   `03-signatures.tex`: The signature page
    -   `04-acknowledgements.tex`: Your acknowledgements
    -   `05-abstract.tex`: Your abstract section
    -   `06-lists.tex`: Table of contents and list of figures & tables
    -   `07-dedication.tex`: You dedication page (optional)

*   All of the chapters are:

    -   `11-chapter-1.tex`: Overview chapter
    -   `12-chapter-2.tex`: Equations of State and our Survey
    -   `13-chapter-3.tex`: Numerical Methods
    -   `14-chapter-4.tex`: Nuclear EOS's in `SpEC`
    -   `15-chapter-5.tex`: Results of our Nuclear EOS Survey

* The bibliography shall be in:

    -   `references/`: Uses `BibTeX` entries 
        ([gscholar.py](https://github.com/venthur/gscholar) is your
	friend)

*   Gnuplot commands to make a vector image with an accompanying tex
    file to include in the manuscript.  On the remote:
    ``` gnuplot
    set terminal epslatex color solid 8
    set output 'images/tov-mass-vs-radius.tex'
    load 'tov-mass-vs-radius.cfg'
    set output
    ```
    As needed, we will add the plot commands to `make-images.cfg` from
    my [gnuplot-scripts](https://github.com/brege/bhns-gnuplot-scripts)
    repo and simply do
    ``` bash
    gnuplot make-images.cfg
    ```
    on the remote. Then, to copy the resulting `*.{eps,tex}` files from
    the remote to the dissertation development folder:
    ``` bash
    ./sync-commands
    ```
