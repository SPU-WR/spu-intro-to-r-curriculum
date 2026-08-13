# Introduction to R Programming at Seattle Public Utilities (SPU)
A list of resources for learning R at SPU


# R

<details>
 
## Core textbooks
* [R for Data Science (2e)](https://r4ds.hadley.nz/)
* [R Packages (2e)](https://r-pkgs.org/)

## Core `R` packages
* [Tidyverse](https://tidyverse.org/)
  * [readr](https://readr.tidyverse.org/) - load rectangular data (`csv` and txt` files)
  * [dplyr](https://dplyr.tidyverse.org/) - manipulate and summarise data
  * [lubridate](https://lubridate.tidyverse.org/) - manipulate dates and times
  * [ggplot2](https://ggplot2.tidyverse.org/) - plot data
* [quarto](https://quarto.org/) - reproducible reporting
* [USGS Data Retrieval](https://doi-usgs.github.io/dataRetrieval/) - query USGS data

## Core concepts
* Data Wrangling
  * [Split-Apply-Combine](https://vita.had.co.nz/papers/plyr.pdf)
* Data Visualization
  * [Best Practices for Data Visualization](https://royal-statistical-society.github.io/datavisguide/)

## Helpful cheatsheets
* [Posit Cheatsheet Library](https://rstudio.github.io/cheatsheets/)
  * In order of importance: Data import with `tidyverse` (loading data), `dplyr` (data wrangling), `ggplot2` (data viz), `lubridate` (date handling), `Quarto` (reporting) 

## Useful blog posts
* [Project-oriented workflow](https://tidyverse.org/blog/2017/12/workflow-vs-script/)
* [USGS Water Data for the Nation Blog](https://waterdata.usgs.gov/blog/)
  * Reproducible Data Science in R series
    * [Writing functions that work for you](https://waterdata.usgs.gov/blog/rds-functions-that-work-for-you/)
    * [Writing better functions](https://waterdata.usgs.gov/blog/rds-better-functions/)
    * [Iterate, don't duplicate](https://waterdata.usgs.gov/blog/rds-iterate/)
    * [Flexible functions using tidy evaluation](https://waterdata.usgs.gov/blog/rds-function-evaluation/)
    * [Say the quiet part out loud with assertion tests](https://waterdata.usgs.gov/blog/rds-assertions/)
  * Reporting
    * [Duplicating Quarto elements with code templates to reduce copy and paste errors](https://waterdata.usgs.gov/blog/quarto-template-demo/)
    * [Principles of Plain Language](https://digital.gov/guides/plain-language/principles)
  * Data Viz
    * [Jazz up your ggplots!](https://waterdata.usgs.gov/blog/ggplot-jazz/)
    * [Friends Don't Let Friends Make Bad Graphs](https://github.com/cxli233/FriendsDontLetFriends)

## Useful courses
* [STAT 545, Jenny Bryan, University of British Columbia](https://stat545.com/)

## Useful blogs
* [USGS VizLab home](https://water.usgs.gov/vizlab/index.html)

## Entry-level projects
* Water Specific Examples
  * template repos
    * Under development
  * Introductory questions/problem statements
    * Which USGS gages are the oldest in the state? Where are the 10 oldest gages located?
    * How much water passes downstream of Landsburg diversion dam during Landsburg Headworks Annual Maintenance (LHAM)?
    * How does the current water year compare to all other water years? The driest water years? The wettest water years?
      * Expand this analysis to include "WY+1" (i.e., WY2020-2021)
* Other
  * [Data Science in a Box Interactive Tutorials](https://datasciencebox.org/02-interactive-tutorials)


## Advanced topics
* Reproducible pipelines with the `targets` package
  * [targets](https://docs.ropensci.org/targets/) - Function-oriented Make-like declarative workflows for R
  * [The {targets} R package user manual](https://books.ropensci.org/targets/)

</details>


# Version Control with `git` and GitHub

<details>
 
## Core textbooks
* [Chapter 20.1 Git and GitHub in R Packages (2e)](https://r-pkgs.org/software-development-practices.html#sec-sw-dev-practices-git-github)
* [Pro Git](https://git-scm.com/book/en/v2)

## Helpful cheatsheets
* under development

## Useful doc
* Git
  * [git documentation](https://git-scm.dev/doc)
  * [Getting Started - First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)
* GitHub
  * [GitHub Docs](https://docs.github.com/en)
  * [GitHub Flavored Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
* Markdown
  * [Basic Syntax](https://www.markdownguide.org/basic-syntax/)

## Useful blog posts
* [Beyond Basic R - Version Control with Git](https://waterdata.usgs.gov/blog/beyond-basic-git/)

## Useful courses
* [Happy git with R](https://happygitwithr.com/)
* [oh my git](https://ohmygit.org/)  - _not yet vetted_
* [Learn git Branching](https://learngitbranching.js.org/) - _not yet vetted_
* [Learn git. Solve mysteries.](https://www.gitnoir.com/) - _not yet vetted_

</details>
