# UALittleRockTemplate

This is a template for graduate thesis or dissertation using pandoc, LaTEX, and Markdown. You should have a basic understanding of Markdown and LaTEX. 

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

    \<String\> The title of the document. This will be used as the title of the document and in the header.
- subtitle

    \<String\> The subtitle of the document. This will be used as the subtitle of the document.
- author

    \<String\> The author of the document. This will be used as the author of the document.
- PHD

    \<Boolean\> Set to true if the document is a PhD dissertation.
- MA

    \<Boolean\> Set to true if the document is a Master of Art thesis.
- MS

    \<Boolean\> Set to true if the document is a Master of Science thesis.
- font_size

    \<String\>The font size of the document. Set to `10pt`, `11pt` or `12pt`. The default is `12pt`.
- program

    \<String\> The program the author is enrolled in. example: "Computer and information Science"
- department

    \<String\> The department the author is enrolled in. example: "Computer Science"
- college

    \<String\> The college the author is enrolled in. example: "Donaghey College of Science, Technology, Engineering, and Mathematics"
- gradmonthyear
  - month  \<String\> The month and year the author is graduating. example: "May"
  - year    \<Integer> The year the author is graduating. example: 2021
- chair_name

    \<String\> The name of the chair of the committee.
- chair_title

    \<String\> The title of the chair of the committee.
- chair_department

    \<String\> The department of the chair of the committee.
- cochair_name

    \<String\> The name of the co-chair of the committee.
- cochair_title

    \<String\> The title of the co-chair of the committee.
- cochair_department

    \<String\> The department of the co-chair of the committee.
- committee_members
  - name
  - title
  - department
  - university_affiliation
  - employer

    \<String\> The name of the committee member.  
    \<String\> The title of the committee member.  
    \<String\> The department of the committee member.  
    \<String\> The university affiliation of the committee member.  
    \<String\> The employer of the committee member.
- abstract

    \<String\> The abstract of the document.
- bibliography

    \<Path\> The path to the bibliography file. This should be a .bib file.
- csl

    \<Path\> The path to the citation style file. This should be a .csl file.
- acknowledgements

    \<String\> The acknowledgements section of the document.
- dedication
    \<String\> The dedication section of the document.
- protocol_irb_approval

    \<Path\> The path to the IRB approval document.
- lof

    \<Boolean\> Set to true if the document has a list of figures.
- list_of_tables

    \<Boolean\> Set to true if the document has a list of tables.
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

    \<String\> The name of the appendix.  
    \<String\> The content of the appendix


## Credits

Parts of this template were derived from Wandmalfarbe's pandoc-latex-template and can be found here: [https://github.com/Wandmalfarbe/pandoc-latex-template.git](https://github.com/Wandmalfarbe/pandoc-latex-template.git)


