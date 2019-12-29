# {{ cookiecutter.title }}

## Requirements

To render the paper, you will need:

1. pandoc
2. pandoc-citeproc
3. LaTeX
4. Node.js (to use shortcuts via `npm run`)

For more information, take a look at Pandoc's [installation instructions](https://pandoc.org/installing.html).

{% if cookiecutter.use_linter == "y"-%}
Next, install the dependencies for linting:

```
npm i
```
{%- endif %}

## Usage

Within the {{ cookiecutter.directory_name }} directory, run:

```shell
# to generate a PDF
pandoc paper.md --filter pandoc-citeproc -o paper.pdf
# or use this shortcut
npm run pdf

# to generate a Word file
pandoc paper.md --filter pandoc-citeproc -o paper.docx
# or use this shortcut
npm run docx

{% if cookiecutter.use_linter == "y" -%}
# to find possible mistakes in your paper
npm run lint

# to automatically fix these mistakes and prettify the file
npm run
{%- endif %}
```
