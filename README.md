# markdown-cv with [quarto](https://quarto.org/)

Tried to adjust [Simon Heß'](https://github.com/simonheb) nice R Markdown cv for non-R users who compile with quarto. At the end of the day this is all "just" LaTeX, Pandoc, and a tiny bit of R under the hood. Perhaps, this is useful for someone else adjusting an R Markdown document to a quarto environment.

[original pdf](https://github.com/simonheb/markdown-cv/blob/main/CV-SH.pdf) in rmarkdown

[quarto pdf](quarto/cv.pdf)

[quarto source](quarto/cv.qmd)

Only hiccups:
- the yaml header is slightly different for quarto documents
- quarto does not like the LaTeX package `titlesec` and throws an error which can be addressed in several ways, see [here](https://github.com/quarto-dev/quarto-cli/issues/6598).
- quarto by default compiles with xelatex, but can be changed to pdflatex (or one adjusts margins to exactly fit table)
- install R and the scholar package (takes a few min for a non-R user)
