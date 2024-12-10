---
# ========================================= #
# Thesis/Dissertation Details - REQUIRED    #
# ========================================= #
title: "TITLE OF YOUR THESIS OR DISSERTATION:"
subtitle: "SECOND PART OF THE TITLE IF APPLICABLE"
author: "Author OfDocument"

# ========================================= #
# Degree Information - REQUIRED             #
# ========================================= #
PHD: true                                               # Set to true for PhD or Comment out
# MA: false                                             # Uncomment and set true if pursuing MA
# MS: false                                             # Uncomment and set true if pursuing MS

# ========================================= #
# Document Formatting - REQUIRED            #
# ========================================= #
font_size: 12pt                                         # Font size for the document

# ========================================= #
# Institution Details - REQUIRED            #
# ========================================= #
program: "Name of the Program"                          # Your program name
department: "Department Name"                           # Your department
college: "College Name"                                 # College affiliation

# ========================================= #
# Graduation Date - REQUIRED                #
# ========================================= #
gradmonthyear: 
  month: December                                       # Graduation month
  year: 2024                                            # Graduation year

# ========================================= #
# Chair/Co-chair Details                    #
# ========================================= #
chair_name: "Chair Name"                                # Required
chair_title: "Professor Title"                          # Required
chair_department: "Professor Department Name"           # Required

cochair_name: "Some Co-chair"                           # Optional
cochair_title: "Professor Title"                        # Optional
cochair_department: "Co-chair Department"               # Optional

# ========================================= #
# Committee Details                         #
# ========================================= #
committee_members:
  - name: "Dr. Alice Smith"                             # Member details - If member is from another University
    title: "Professor"                                
    department: "Department of Computer Science"      
    university_affiliation: "University of Arkansas"
  - name: "Dr. Bob Johnson"                             # Member details - If from UA Little Rock
    title: "Associate Professor"
    department: "Department of Mathematics"
  - name: "Jane Doe"                                    # Member details - If an expert from industry
    title: "Data Scientist"
    employer: "Tech Solutions Inc."

# ========================================= #
# Abstract Section  - REQUIRED              #
# ========================================= #
abstract: |
  Replace this text with the text of your abstract. The abstract must be double-spaced. There is no word limit for the abstract. To help people find your research, please make sure that the abstract contains a summary of all the key components of your work: the problem statement, the purpose of the research, the methodology, the results, and the analysis or implications of the research.

# ========================================= #
# References/Bibliography - REQUIRED        #
# ========================================= #
bibliography: ['references/references.bib']             # Enter the p[ath to the Biblatex file
csl: references/ieee.csl                                # Enter the path to the Citation Style Language

# ========================================= #
# Optional/Required if Applicable           #
# ========================================= #
acknowledgements: >
  This is an acknowledgements section to all that blah blah. (Replace with your acknowledgements text.)

dedication: >
  This is a dedication to all that blah blah. (Replace with your dedication text.)

protocol_irb_approval: example.pdf                      # Path to the pdf. Comment out if not needed
lof: true                                               # List of figures: Set to false or comment if not needed
list_of_tables: true                                    # List of tables: Set to false or comment out if not needed

list_of_symbols:
  abbreviation:                                         # Optional: Only needed if abbreviation is not spelled out in content of document.
    - key: CPU                                          # Abbreviation
      value: Central Processing Unit                    # Meaning of Abbreviation
    - key: RAM
      value: Random Access Memory
  symbols:                                              # Optional: Only utf-8 supported
    - key: "µ"                                          # Symbol
      value: Mu                                         # Meaning of Symbol
    - key: "ß"
      value: Beta
  nomenclature:                                         # Optional
    - key: Algorithm                                    # First word
      value: A step-by-step procedure for calculations  # Definition of the key word
    - key: Data Structure
      value: A particular way of organizing data in a computer

appendix:                                               # Optional: Only required if adding appendix
  - name: "Appendix A"                                  # Name of the appendix
    content: |                                          # Content of the appendix
      This is the content for Appendix A.
  - name: "Appendix B"
    content: |
      This is the content for Appendix B.

---

# First Section - Heading 1 

This document is a template for writing a thesis or dissertation using markdown. The template is based on the official guidelines from the University of Arkansas at Little Rock. Below are some examples of how to use the template. You can add references to the references.bib file and use the citation keys in the document [@wing]. The reference is placed using the `[@name_of_reference]` syntax.

To use this document it is recommended that you understand the basics of markdown. The document is divided into sections and subsections. The sections are denoted by the `#` symbol followed by the section title. Subsections are denoted by the `##` symbol followed by the subsection title. for more help with markdown, you can visit the [https://www.markdownguide.org/](https://www.markdownguide.org/).

## Tables and Figures - Heading 2

: Sample Grid table.

+------------+------------+-----------------------+------------+------------+------------------------+
| Fruit      | Price      | Advantages            | Fruit      | Price      | Advantages             |
+============+============+=======================+============+============+========================+
| Bananas    | $1.34      | * built-in wrapper    | Bananas    | $1.34      |   built-in wrapper     |
|            |            | * bright color        |            |            |   bright color         |
+------------+------------+-----------------------+------------+------------+------------------------+
| Oranges    | $2.10      | cures scurvy          | Oranges    | $2.10      |   cures scurvy         |
|            |            | tasty                 |            |            |   tasty                |
+------------+------------+-----------------------+------------+------------+------------------------+

: Sample Pipe Table

| Right | Left | Default | Center |
|------:|:-----|---------|:------:|
|   12  |  12  |    12   |    12  |
|  123  |  123 |   123   |   123  |
|    1  |    1 |     1   |     1  |

| Right | Left | Default | Center |
|------|-----|---------|------|
|   12  |  12  |    12   |    12  |
|  123  |  123 |   123   |   123  |
|    1  |    1 |     1   |     1  |

: Sample Table with Caption

## Code Block Example

```sh
ls -la
```

## Math

### Inline Math - Heading 3

This sentence uses `$` delimiters to show math inline: $\sqrt{3x-1}+(1+x)^2$
This sentence uses `$` delimiters to show math inline: $\sqrt{3x-1}+(1+x)^2$

### Latex Math - Heading 3

  $$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

## Figures - Heading 2

To place a figure in the document, you can use the following syntax. The figure is placed using the `![Caption](path_to_image)` syntax.

![Sample figure](img/ua-little-rock.png)

## Lists - Heading 2

### Unordered List - Heading 3

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

### Ordered List - Heading 3

1. Item 1
2. Item 2
   1. Item 3
   2. Item 4
   3. Item 5
3. Item 6

### Section 1.2.1

Donec vitae sapien ut libero venenatis faucibus. Nullam quis ante. Etiam sit amet orci eget eros faucibus tincidunt. Duis leo. Sed fringilla mauris sit amet nibh. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada.



# Section 2

Phasellus viverra nulla ut metus varius laoreet. Quisque rutrum. Aenean imperdiet. Etiam ultricies nisi vel augue. Curabitur ullamcorper ultricies nisi. Nam eget dui. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. 

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada.

## Section 2.1

Etiam rhoncus. Maecenas tempus, tellus eget condimentum rhoncus, sem quam semper libero, sit amet adipiscing sem neque sed ipsum. Nam quam nunc, blandit vel, luctus pulvinar, hendrerit id, lorem. Maecenas nec odio et ante tincidunt tempus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lacinia odio vitae vestibulum vestibulum. Cras venenatis euismod malesuada.

\newpage
# References