# Resume / CV LaTeX Source

This repository contains the LaTeX source for a resume and a longer CV. The main documents are assembled from small section files so individual entries can be updated without editing the full document.

## Project Tree

```text
.
├── cv.tex
├── resume.tex
├── skills.tex
├── education/
│   ├── university-of-michigan.tex
│   └── western-high-school.tex
├── experience/
│   ├── ally-1.tex
│   ├── ally-2.tex
│   ├── center-lake-fitness.tex
│   └── michigan-soccer-referee-association.tex
├── research/
│   ├── university-of-michigan-1.tex
│   └── university-of-michigan-2.tex
├── projects/
│   ├── fps-pvp-dynamics.tex
│   ├── photo-processing-helper.tex
│   └── predicting-survival-in-the-icu.tex
├── resume.pdf
├── cv.pdf
└── .github/, .vscode/, .gitignore, and other repo/config files
```

## Important Files

`resume.tex` is the shorter, application-focused version of the document. It includes education, work experience, research, projects, and a skills section.

`cv.tex` is the longer curriculum vitae version. It includes a summary section and a broader set of work and research entries than the resume.

`skills.tex` contains the skills table that is reused by both documents.

## Directories

`education/` holds individual education entries that are inserted into the main documents with `\input{...}`.

`experience/` contains work entries. The main `.tex` files decide which of these entries appear in the resume or CV.

`research/` contains the research experience entries that are inserted into the main documents with `\input{...}`.

`projects/` contains project descriptions that are included in the final documents.

## Generated Files

`resume.pdf` and `cv.pdf` are the compiled outputs. They are generated from `resume.tex` and `cv.tex` respectively.

## Editing Workflow

To update a section, edit the corresponding file in `education/`, `experience/`, `projects/`, or `skills.tex`, then recompile the relevant top-level `.tex` file.