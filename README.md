# Carleton University Thesis Template 

This repository provides a Typst-based thesis template for Carleton University students. It is designed for simplicity and modularity, allowing you to easily structure your thesis into separate chapters while keeping configuration details in one place.

## Project Structure

```
├── chapters/               # Write each section of your thesis here
│   ├── abstract.typ
│   ├── acknowledgements.typ
│   ├── background.typ
│   ├── conclusion.typ
│   ├── discussions.typ
│   ├── introduction.typ
│   ├── methodology.typ
│   ├── results.typ
│   └── title.typ
├── figures/                # Store all thesis figures/images here
├── config.typ              # Configuration file (title, author, degree, examiners, etc.)
├── main.pdf                # Rendered PDF
├── main.typ                # Entry point 
├── ref.bib                 # Bibliography file (BibTeX format)
└── README.md               
```

## Configuration

Edit `config.typ` to update your thesis details:

```
#let thesis_title = "Lorem Thesis Title"
#let thesis_subtitle = "The details of Ipsum"
#let name = "Justin Zhang"
#let degree = "Masters of Computer Science"
#let degree_program = "Master of Computer Science (Data Science)"
#let examiners = (
  "Dr. Olga Baysal, Thesis Supervisor",
  "Dr. Suess, Author",
  "Dr. Mario, Plumber",
  "Dr. Who, Time Traveller",
  "Dr. Strange, Neurosurgeon",
)
```

## Writing Your Thesis
- Write each section in its corresponding file inside the `chapters/` folder.
- Add figures/images to the `figures/` folder and reference them in your chapters.
- Manage citations in `ref.bib` using standard BibTeX format.

The `main.typ` file automatically assembles everything, so no need to edit it.

## Compiling

You can build the thesis in two ways:

### 1. Using Typst CLI 

```
typst compile main.typ
```

This generates a PDF of your thesis

### Using Typst's Web App

Alternatively, upload the project to the [Typst web application](https://typst.app) and view your thesis directly in the browser.

## License

This template is distributed under [MIT](LICENSE.md)

