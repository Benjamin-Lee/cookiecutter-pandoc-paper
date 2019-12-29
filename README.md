# cookiecutter-pandoc-paper

A [Cookiecutter](https://github.com/cookiecutter/cookiecutter) for writing papers in Markdown via Pandoc.

## Features

- Use either one or two column layout
- Support for double spacing and line numbering
- Customizable font size and margins
- APA, AMA, MLA, CMS, IEEE, Nature, and ACS citation styles out of the box
- Grammar checking (and fixing!) via [Textlint](https://textlint.github.io)
- Preconfigured scripts for PDF and Word file generation (via `npm run pdf` and `npm run docx`)

## Usage

First, you will need to have [installed Cookiecutter](https://cookiecutter.readthedocs.io/en/1.7.0/installation.html):

```shell
# using pip
pip install cookiecutter

# on a Mac
brew install cookiecutter

# using Conda
conda config --add channels conda-forge && conda install cookiecutter
```

Then, use Cookiecutter to scaffold the paper:

```shell
cookiecutter gh:Benjamin-Lee/cookiecutter-pandoc-paper
```
