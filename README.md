# markdown-cv with quarto 

Tried to adjust [Simon Heß'](https://github.com/simonheb) nice R [Markdown cv](https://github.com/simonheb/markdown-cv) for non-R (studio) users who compile with [quarto](https://quarto.org/). At the end of the day this is all "just" LaTeX, Pandoc, and a tiny bit of R under the hood. Perhaps, this is useful for someone else adjusting an R Markdown document to a quarto environment.

PDF: [Original R Markdown](https://github.com/simonheb/markdown-cv/blob/main/CV-SH.pdf), [Quarto version](quarto/cv.pdf)

Source: [Original R Markdown](https://github.com/simonheb/markdown-cv/blob/main/CV-SH.pdf), [Quarto version](quarto/cv.qmd)

Only hiccups:
- change filename extension from .rmd to .qmd
- the yaml header is slightly different for quarto documents
- quarto does not like the LaTeX package `titlesec` and throws an error which can be addressed in several ways, see [here](https://github.com/quarto-dev/quarto-cli/issues/6598).
- quarto by default compiles with xelatex, but that can be changed to pdflatex (or one adjusts margins to exactly fit the table structure)
- install R and the scholar package (takes a few min for a non-R user)
