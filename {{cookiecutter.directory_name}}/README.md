# {{ cookiecutter.title }}

## Requirements

To render the paper, you will need:

1. pandoc
2. pandoc-citeproc
3. LaTeX

For more information, take a look at Pandoc's [installation instructions](https://pandoc.org/installing.html).

## Usage

Within the {{ cookiecutter.directory }} directory, run:

```shell
# to generate a PDF
pandoc paper.md --filter pandoc-citeproc -o paper.pdf

# to generate a Word file
pandoc paper.md --filter pandoc-citeproc -o paper.docx
```
