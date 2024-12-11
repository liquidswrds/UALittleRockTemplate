# UA Little Rock Dissertation/Thesis Template

Welcome to the UA Little Rock Dissertation/Thesis Template repository! This project provides a LaTeX template designed for graduate students at the University of Arkansas at Little Rock who are writing a dissertation or thesis. The template is compatible with Pandoc, enabling easy conversion of Markdown files into high-quality PDF documents.

## Repository URL

[UALittleRockTemplate GitHub Repository](https://github.com/liquidswrds/UALittleRockTemplate.git)

## Features

- **University-specific styling:** Adheres to UA Little Rock formatting guidelines for dissertations and theses.
- **Markdown to PDF conversion:** Write your content in Markdown for simplicity and let Pandoc handle the conversion to LaTeX and PDF.
- **Customizable structure:** Easily modify the template to suit your specific needs while maintaining academic standards.
- **Cross-platform support:** Works on Windows, macOS, and Linux.

## Getting Started

### Prerequisites

- **Pandoc:** Install Pandoc for Markdown to LaTeX conversion. Visit the [Pandoc website](https://pandoc.org/) for installation instructions.
- **LaTeX Distribution:** Ensure you have a LaTeX distribution installed (e.g., TeX Live, MikTeX, or MacTeX).

### Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/liquidswrds/UALittleRockTemplate.git
   ```

2. Navigate to the project directory:

   ```sh
   cd UALittleRockTemplate
   ```

## Usage

1. Write your content in Markdown format (e.g., `example_document.md`).
2. Use the provided LaTeX template to convert the Markdown file into a PDF.

   Example command:

   ```bash
   pandoc -s -o test.pdf --template=ua_little_rock.tex example_document.md --citeproc
   ```

3. Review and refine the generated PDF to ensure compliance with UA Little Rock formatting guidelines.

## YAML Variables for UA Little Rock Dissertation/Thesis Template

Below is a detailed explanation of the YAML variables used in the template. Each variable includes its type, explanation, and an example of how it can be used.

### Thesis/Dissertation Details

#### `title` (Type: string)

- **Description:** The title of your thesis or dissertation.
- **Example:**
  
  ```yaml
  title: "Exploring Artificial Intelligence in Education"
  ```

#### `subtitle` (Type: string, optional)

- **Description:** A second part of the title, if applicable.
- **Example:**

  ```yaml
  subtitle: "Applications and Implications"
  ```

#### `author` (Type: string)

- **Description:** The name of the author (you).
- **Example:**

  ```yaml
  author: "Jane Doe"
  ```

### Degree Information

#### `PHD` (Type: boolean)

- **Description:** Set to `true` if pursuing a PhD; otherwise, comment out.
- **Example:**

  ```yaml
  PHD: true
  ```

#### `MA` or `MS` (Type: boolean, optional)

- **Description:** Uncomment and set to `true` for Master of Arts or Master of Science.
- **Example:**

  ```yaml
  MS: true
  ```

### Document Formatting

#### `font_size` (Type: int)

- **Description:** The font size for the document text.
- **Example:**

  ```yaml
  font_size: 12pt
  ```

### Institution Details

#### `program` (Type: string)

- **Description:** The name of your academic program.
- **Example:**

  ```yaml
  program: "Computer Science"
  ```

#### `department` (Type: string)

- **Description:** The name of your department.
- **Example:**

  ```yaml
  department: "Department of Computer Science"
  ```

#### `college` (Type: string)

- **Description:** The name of your college.
- **Example:**

  ```yaml
  college: "College of Engineering and Information Technology"
  ```

### Graduation Date

#### `gradmonthyear` (Type: object)

- **Description:** Specifies your graduation month and year.
- **Example:**

  ```yaml
  gradmonthyear:
    month: May
    year: 2025
  ```

### Chair/Co-chair Details

#### `chair_name`, `chair_title`, `chair_department` (Type: string)

- **Description:** Information about your chairperson.
- **Example:**

  ```yaml
  chair_name: "Dr. John Smith"
  chair_title: "Professor"
  chair_department: "Department of Computer Science"
  ```

#### `cochair_name`, `cochair_title`, `cochair_department` (Type: string, optional)

- **Description:** Information about your co-chairperson, if applicable.
- **Example:**

  ```yaml
  cochair_name: "Dr. Alice Johnson"
  cochair_title: "Associate Professor"
  cochair_department: "Department of Mathematics"
  ```

### Committee Details

#### `committee_members` (Type: list of objects)

- **Description:** Information about your committee members, including their name, title, department, and affiliation.
- **Example:**

  ```yaml
  committee_members:
    - name: "Dr. Alice Smith"
      title: "Professor"
      department: "Department of Computer Science"
      university_affiliation: "University of Arkansas"
    - name: "Dr. Bob Johnson"
      title: "Associate Professor"
      department: "Department of Mathematics"
  ```

### Abstract Section

#### `abstract` (Type: string)

- **Description:** A summary of your research, including problem statement, methodology, results, and analysis.
- **Example:**

  ```yaml
  abstract: |
    This study explores the applications of artificial intelligence in modern education.
    It analyzes the implications of AI-driven tools on learning outcomes.
  ```

### References/Bibliography

#### `bibliography` (Type: list of strings)

- **Description:** Path(s) to your BibLaTeX file(s).
- **Example:**

  ```yaml
  bibliography: ['references/references.bib']
  ```

#### `csl` (Type: string)

- **Description:** Path to the Citation Style Language file.
- **Example:**

  ```yaml
  csl: references/ieee.csl
  ```

### Optional Sections

#### `acknowledgements` (Type: string, optional)

- **Description:** Acknowledgements section text.
- **Example:**

  ```yaml
  acknowledgements: |
    I would like to thank my family and mentors for their support.
  ```

#### `dedication` (Type: string, optional)

- **Description:** Dedication section text.
- **Example:**

  ```yaml
  dedication: |
    This work is dedicated to my parents.
  ```

#### `list_of_symbols` (Type: object, optional)

- **Description:** Abbreviations, symbols, and nomenclature used in the document.
- **Example:**

  ```yaml
  list_of_symbols:
    abbreviation:
      - key: CPU
        value: Central Processing Unit
    symbols:
      - key: "µ"
        value: Mu
  ```

#### `appendix` (Type: list of objects, optional)

- **Description:** Appendices included in the document.
- **Example:**

  ```yaml
  appendix:
    - name: "Appendix A"
      content: |
        This is the content for Appendix A.
    - name: "Appendix B"
      content: |
        This is the content for Appendix B.
  ```

## Repository Structure

```sh
UALittleRockTemplate/
├── LICENSE                # License file
├── README.md              # Documentation (this file)
├── example                # Example output directory
│   └── test.pdf           # Example generated PDF
└── template               # Template and supporting files
    ├── example_document.md # Example Markdown file
    ├── img                 # Image assets
    │   └── ua-little-rock.png # UA Little Rock logo
    ├── references          # References and citation styles
    │   ├── chicago-fullnote.csl
    │   ├── chicago-note.csl
    │   ├── ieee.csl
    │   └── references.bib
    └── ua_little_rock.tex  # LaTeX template
```

## Contributing

We welcome contributions to improve the template. If you encounter issues or have suggestions, please submit them via the [Issues](https://github.com/liquidswrds/UALittleRockTemplate/issues) tab. For direct contributions:

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Submit a pull request.

## License

This repository is licensed under the [Apache License 2.0](LICENSE). You are free to use, modify, and distribute the template as long as proper attribution is provided.

## Support

For questions or support, please open an issue in the repository.

## Acknowledgments

Parts of this template were derived from Wandmalfarbe's pandoc-latex-template and can be found here: [https://github.com/Wandmalfarbe/pandoc-latex-template.git](https://github.com/Wandmalfarbe/pandoc-latex-template.git)

Special thanks to the University of Arkansas at Little Rock for their academic resources and to the open-source community for tools like Pandoc and LaTeX.

