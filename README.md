# UALittleRockTemplate

This is a template for graduate thesis or dissertation using pandoc, LaTEX, and Markdown. You should have an basic understanding of Markdown and LaTEX. 

If you are looking for information on Markdown: [Markdown Guide](https://www.markdownguide.org/)
If you are looking for information on LaTEX: [LaTEX Wiki](https://en.wikibooks.org/wiki/LaTeX)
If you are looking for information on pandoc: [Pandoc User Guide](https://pandoc.org/MANUAL.html)

## Installation

Download this repository to your computer.

```sh
git clone https://github.com/liquidswrds/UALittleRockTemplate.git
```


## Usage

To use this template, you need to have pandoc and LaTEX installed on your computer. Plkease refer to the installation guide for pandoc [https://pandoc.org/installing.html](https://pandoc.org/installing.html)

To compile the document, you can use the following command:

```sh
pandoc -s -o output.pdf --template=ua_little_rock.tex example_document.md --citeproc
```

This command will compile the example_document.md into a PDF file called output.pdf. The --citeproc flag is used to enable citation processing.

## YAML Variables

The template uses YAML variables to set the title, author, and other information. The YAML block should be at the beginning of the document and should be enclosed by three dashes. 

- title
- subtitle
- author
- PHD
- MA
- MS
- font_size
- program
- department
- college
- gradmonthyear
  - month
  - year
- chair_name
- chair_title
- chair_department
- cochair_name
- cochair_title
- cochair_department
- committee_members
  - name
  - title
  - department
  - university_affiliation
  - employer
- abstract
- bibliography
- csl
- acknowledgements
- dedication
- protocol_irb_approval
- lof
- list_of_tables
- list_of_symbols
  - abbreviation
    - key
    - value
  - symbols
    - key
    - value
  - nomenclature
    - key
    - value
- appendix
  - name
  - content


## Credits

Parts of this template were derived from Wandmalfarbe's pandoc-latex-template and can be found here: [https://github.com/Wandmalfarbe/pandoc-latex-template.git](https://github.com/Wandmalfarbe/pandoc-latex-template.git)


