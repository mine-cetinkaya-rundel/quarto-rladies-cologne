# quarto-rladies-cologne

Hello, Quarto: A World of Possibilities (for Reproducible Publishing) talk for R-Ladies Cologne

## Setup notes

- RStudio: Version 2023.09.0+463 (2023.09.0+463)
- Quarto: 1.4.395
- R: 4.3.1 (2023-06-16) -- "Beagle Scouts"
- Packages: tidyverse, palmerpenguins, gt

## Demo

### Documents

- Open the simple Quarto document called `index.qmd` and edit it using the RStudio Visual Editor.
- Bold palmerpenguins and add link to https://allisonhorst.github.io/palmerpenguins/.
- Add code chunk options:
  - `fig-alt`
  - `echo: false` in `execute` in the YAML
  - `code-fold`
  - teaching tip: `echo: fenced`
- Add a figure and a table and cross reference them
- Add a citation: 10.1371/journal.pone.0090081

### Slides

- Change `format: revealjs`
- Add section headings: First level headings Introduction and Analysis, under Analysis a second level heading called Modeling
- Incremental lists
- Add columns and tabsets
- Reveal code with `echo: true`
  - teaching-tip: `code-line-numbers`
- Change `output-location` of figure
- Logo and footer
- Making things fit on a slide
- Chalkboard
- Publishing your presentation to Quarto Pub
- Printing to PDF

### Websites

- Add `quarto.yml` 

```
project:
  type: website

website:
  title: "Hello Quarto"
  navbar:
    left:
      - index.qmd
      - talk.qmd
```

- Render
- Add other formats to index.qmd:

```
format:
  html: default
  pdf: default
```

- Navigation
- Add one more document with R chunk
- Freeze
- Themes and dark theme toggle
- `publish quarto`

### Journal articles (time permitting)

- Go to https://quarto.org/docs/journals/templates.html

- Click on Quarto journals repo

- Create one with JASA template

my-awesome-paper

- Add a citation

First from Zotero
Welcome to the tidyverse