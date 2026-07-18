# Repository Instructions

This repository contains LaTeX sources for a resume and CV. Start with [README.md](README.md) for the document layout and editing workflow, then work locally in the smallest file that owns the content.

## What To Edit

- Use [resume.tex](resume.tex) for the short resume content and section ordering.
- Use [cv.tex](cv.tex) for the longer CV content and section ordering.
- Use the files under [education/](education), [experience/](experience), [projects/](projects), [research/](research), and [skills.tex](skills.tex) for entry text.
- Use [resume.cls](resume.cls) only for global formatting, spacing, headers, or shared macros.

## Editing Conventions

- Keep changes narrow and content-driven. Avoid reformatting unrelated LaTeX unless the task is about layout.
- Preserve the existing macro-based structure, especially `\experience`, `bullets`, and `items`.
- Prefer updating a single section file over editing the top-level document when only one entry changes.
- Keep section order intentional; the top-level files decide which entries appear in the resume versus the CV.

## Validation

- Rebuild the affected document after edits. Use `latexmk -pdf resume.tex` for the resume and `latexmk -pdf cv.tex` for the CV.
- Treat [resume.pdf](resume.pdf) and [cv.pdf](cv.pdf) as generated artifacts.

## Agent Notes

- Link to docs instead of duplicating them when possible.
- If you need deeper project context, inspect the main TeX file and the nearest section file first.