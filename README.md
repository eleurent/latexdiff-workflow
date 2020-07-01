# latexdiff-workflow
A [workflow](.github/workflows/latexdiff.yml) to show the diff between two versions of a latex document.

It uses:
* [actions/checkout](https://github.com/actions/checkout) to get the two versions (`master` and `v1` tag) of the latex document
* [latexdiff](https://www.ctan.org/pkg/latexdiff) to generate the difference between the two documents
* [latex-action](https://github.com/xu-cheng/latex-action) to build the pdf from the latex difference file

The result is uploaded as an artifact.
