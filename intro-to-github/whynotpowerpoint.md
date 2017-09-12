% Why not PowerPoint: alternative tools to build and share knowledge

## Statement of purpose

I want a workflow that will cover the following:

* Reference management
* Writing
* Generate output (deliverables)
* Backup and version control

# 1. Reference management

## Requirements

* File management:
    * Store (or manage storage of) PDF files, consistent/meaningful file naming
    * Allow cloud-storage for _portable_ access (e.g. reading from a tablet) 

----------

* File management:
    * Store (or manage storage of) PDF files, consistent/meaningful file naming
    * Allow cloud-storage for _portable_ access (e.g. reading from a tablet) 
* Citations
    *  Easily cite references

## Tool of choice

![[Mendeley](https://www.mendeley.com)](img/mendeley.jpg)

---------

![Screenshot from Mendeley](img/mendeley-screenshot.png)

----------

![Highlighting PDF files, exporting to plain text with [Sumnotes](https://www.sumnotes.net/)](img/highlights-sumnotes.png)

# 2. Writing

## Requirements

* Allow for distraction-free writing
* Citations: easily cite references
* Avoid platform dependencies
* Avoid file corruption

# 3. Output/deliverables

## Requirements

* Escape the need to spend time on formatting
* Ease or make format transformations more flexible
* Citations: easily cite references

# Swiss-Army Knife for tasks 2 & 3

## Tool of choice

![[Pandoc](http://pandoc.org/)](img/pandoc.png) 

--------

Pandoc for writing and formatting: 

one tool to work on the two of them separately

--------

![Plain text writing](img/sublime-screenshot.png)

--------

### Pandoc commands

Generate a PDF output (`-o target-filename.pdf`) from Markdown source (`src-filename.md`), typographically correct (`-S`), standalone (`-s`), with numbered sections (`-N`), taking bibliographic references from the specified BibTeX file (`--bibliography=library.bib`).

```
pandoc -S -s -N --bibliography=library.bib  
    -o target-filename.pdf src-filename.md
```

-------

### Pandoc commands

Generate a Word output (`-o target-filename.docx`) from Markdown source (`src-filename.md`), standalone (`-s`), taking bibliographic references from the specified BibTeX file (`--bibliography=library.bib`).

```
pandoc -s --bibliography=library.bib 
    -o target-filename.docx src-filename.md
```

--------

One source-file to produce-them-all (outputs):

![PDF through LaTeX _vs._ Word](img/pandoc-outputs.png)

## Main advantage

* Single source file, multiple outputs
* Simplified writing markup: [Markdown](http://daringfireball.net/projects/markdown/) _vs._ raw [LaTeX](http://www.latex-project.org/)

---------

![LaTex source screenshot](img/latex-screenshot.png)

---------

Markdown syntax is simple and easy to remember

![Sample of Markdown syntax](img/markdown-example.png)

---------

Pandoc makes it more practical for academic purposes. 

Adds support for:

* Metadata blocks (simple or YAML-formatted)
* Internal and reference links

------

And, more importantly,

* Footnotes
```
    Here is a footnote reference,[^1] 
    and another.[^longnote]

    [^1]: Here is the footnote.

    [^longnote]: Here's one with multiple blocks.

      Subsequent paragraphs are indented to show
      that they belong to the previous footnote.
```

------

* Citations
```
    Blah blah [see @doe99, pp. 33-35; also @smith04, ch. 1].

    Blah blah [@smith04; @doe99].

    Smith says blah [-@smith04].

    @smith04 says blah.

    @smith04 [p. 33] says blah.
```

## Bonus:

### Advanced plain-text editor

----

![[Sublime Text](http://www.sublimetext.com/): pleasant to write in, efficient to revise and build](img/st2.png)

# 4. Backup and version control

## Requirements

* Give peace of mind (avoid panic-attacks at all points)
* Allow restoration to previous versions without losing integrity
* Function with minimum human intervention (prone to errors)

## Tool of choice

![[Github](https://github.com/)](img/github.png)

## Bonus:

### Do research with Open Access at the same time

* Data and research process can be available for everyone (or at least for some)
* Allows reproducibility, leads to increased dissemination and greater social impact
* It is the right thing to do

This presentation, hosted on Github: 
http://mrn.bz/whynotpowerpoint

Repository for this presentation: 
http://mrn.bz/whynotpowerpoint-repo

# Thanks!

### Miren Berasategi

@[mberasategi](http://twitter.com/mberasategi)

[miren.berasategi@deusto.es](mailto:miren.berasategi@deusto.es) 

[http://d.mberasategi.com](http://d.mberasategi.com)
