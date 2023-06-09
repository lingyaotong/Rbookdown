Welcome!

This is a minimal example of a book based on R Markdown and **bookdown** (<https://github.com/rstudio/bookdown>).

This template provides a skeleton file structure that you can edit to create your book.

The contents inside the .Rmd files provide some pointers to help you get started, but feel free to also delete the content in each file and start fresh.

Additional resources:

The **bookdown** book: <https://bookdown.org/yihui/bookdown/>

The **bookdown** package reference site: <https://pkgs.rstudio.com/bookdown>


##Update all your R and LaTeX packages:##
update.packages(ask = FALSE, checkBuilt = TRUE)
tinytex::install_tinytex()
tinytex::tlmgr_update()

##install R-bookdown
devtools::install_github('rstudio/bookdown')

##get started##
title: "lingyaotong"
author: "佟玲瑶"
date: "`r Sys.Date()`"
site: bookdown::bookdown_site
documentclass: book
bibliography: [book.bib, packages.bib]
# url: your book url like https://bookdown.org/yihui/bookdown
# cover-image: path to the social sharing image like images/cover.jpg
description: |
  This is a minimal example of using the bookdown package to write a book.
  The HTML output format for this example is bookdown::gitbook,
  set in the _output.yml file.
link-citations: yes
github-repo: rstudio/bookdown_lingyao


bookdown::render_book("index.Rmd", 
  output_format="bookdown::gitbook", encoding="UTF-8")