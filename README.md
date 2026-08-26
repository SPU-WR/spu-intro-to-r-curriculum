# Introduction to R Programming at Seattle Public Utilities (SPU)
A list of resources for learning R at SPU

> It’s easy when you start out programming to get really frustrated and think, “Oh it’s me, I’m really stupid,” or, “I’m not made out to program.” But, that is absolutely not the case. Everyone gets frustrated. I still get frustrated occasionally when writing R code. It’s just a natural part of programming. So, it happens to everyone and gets less and less over time. Don’t blame yourself. Just take a break, do something fun, and then come back and try again later.

[Hadley Wickham](https://r-posts.com/advice-to-young-and-old-programmers-a-conversation-with-hadley-wickham/)

# R

<details>
 
## Core textbooks
* [R for Data Science (2e)](https://r4ds.hadley.nz/)
* [R Packages (2e)](https://r-pkgs.org/)

## Core `R` packages
* [Tidyverse](https://tidyverse.org/)
  * [readr](https://readr.tidyverse.org/) - load rectangular data (`csv` and `txt` files)
  * [tidyr](https://tidyr.tidyverse.org/) - tidy messy data
  * [dplyr](https://dplyr.tidyverse.org/) - manipulate and summarise tidy data
  * [lubridate](https://lubridate.tidyverse.org/) - manipulate dates and times
  * [ggplot2](https://ggplot2.tidyverse.org/) - plot data using a layered approach
* [quarto](https://quarto.org/) - reproducible reporting
* [USGS Data Retrieval](https://doi-usgs.github.io/dataRetrieval/) - query USGS data
* Geospatial packages
  * [sf](https://r-spatial.github.io/sf/reference/sf-package.html) - a standardized way to encode and analyze spatial vector data (vectors only)
  * [terra](https://rspatial.github.io/terra/index.html) - spatial data handling (both rasters and vectors)

## Core concepts
* Data Wrangling
  * [Tidy Data (Wickham, 2014)](https://vita.had.co.nz/papers/tidy-data.pdf)
  * [Split-Apply-Combine (Wickham, 2011)](https://vita.had.co.nz/papers/plyr.pdf)
  * [Don't Repeat Yourself (DRY)](https://lawsofsoftwareengineering.com/laws/dry-principle/)
* Workflow Management & Documentation
  * [Project-oriented workflows (Bryan, 2017)](https://tidyverse.org/blog/2017/12/workflow-vs-script/)
  * [Principles of Plain Language](https://guides.18f.org/content-guide/our-approach/plain-language/)
* Data Visualization
  * [A Layered Grammar of Graphics (Wickham, 2010)](https://vita.had.co.nz/papers/layered-grammar.pdf)
  * [Best Practices for Data Visualization](https://royal-statistical-society.github.io/datavisguide/)

## Helpful cheatsheets
* [Posit Cheatsheet Library](https://rstudio.github.io/cheatsheets/)
  * In order of importance: Data import with `tidyverse` (loading data), `tidyr` (tidy messy data), `dplyr` (data wrangling), `ggplot2` (data viz), `lubridate` (date handling), `Quarto` (reporting) 

## Useful blog posts
* [USGS Water Data for the Nation Blog](https://waterdata.usgs.gov/blog/)
  * Beyond Basic R series
    * [The case for reproducibility](https://waterdata.usgs.gov/blog/reproducibility/)
    * [Introduction and Best Practices](https://waterdata.usgs.gov/blog/intro-best-practices/)
    * [Version Control with Git](https://waterdata.usgs.gov/blog/beyond-basic-git/) - _this is in the `git` section below, but I think it's worth introducing the topic up here_
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
* [R Crash Course](https://r-crash-course.github.io/) - Introduction to R for non-programmers using gapminder data
* [STAT 545, Jenny Bryan, University of British Columbia](https://stat545.com/) - A course dedicated to everything that comes up during data analysis with R __except__ for statistical modelling and inference (i.e., data wrangling, exploration, and analysis)
* [Write Efficient Scientific Code - the DRY (Don’t Repeat Yourself) Principle](https://earthdatascience.org/courses/earth-analytics/automate-science-workflows/write-efficient-code-for-science-r/) - course aimed at applying DRY principles to code development
* [Fred Hutch Data Science Courses](https://ocdo.fredhutch.org/dasl/courses/) - available as self-guided resources
  * [Intro to R](https://hutchdatascience.org/Intro_to_R/) - _not vetted_ Uses the Posit Cloud Workspace
  * [Intermediate R](https://ocdo.fredhutch.org/dasl/courses/intermediate-r/) - _not vetted_ Uses the Posit Cloud Workspace

## Useful blogs
* [USGS Water Data for the Nation Blog](https://waterdata.usgs.gov/blog/)
* [USGS VizLab home](https://water.usgs.gov/vizlab/index.html)
* [Fred Hutch Biomedical Data Science Wiki](https://sciwiki.fredhutch.org/datademos/)
  
## Entry-level projects
* Water Specific Examples - all entry-level projects should be completed using a [project-oriented workflow](https://tidyverse.org/blog/2017/12/workflow-vs-script/)
  * template repos
    * Under development
  * Introductory questions/problem statements
    * Find and analyze 50-years of daily streamflow for the following USGS gages: 12114500, 12117500, 12117600, 12147600, 12148000, 12148300. Plot the median streamflow for each gage and month of the year for that period.
    * Which USGS gages are the oldest in the state? Where are the 10 oldest gages located?
    * How much water passes downstream of Landsburg diversion dam during Landsburg Headworks Annual Maintenance (LHAM)?
    * How does the current water year compare to all other water years? The driest water years? The wettest water years?
      * Expand this analysis to include "WY+1" (i.e., WY2020-2021)
    * Find and analyze SNOTEL data for the following sites: Cougar Mountain (420), Meadows Pass (897), Tinkham Creek (899), Mount Gardner (898), Stevens Pass (791), Stampede Pass (788), Olallie Meadows (672), Skookum Creek (912), Rex River (911)
      * Which station receives the most snow?
      * How does snowfall this water year compare to other water years?
* Other
  * [Data Science in a Box Interactive Tutorials](https://datasciencebox.org/02-interactive-tutorials)


## Advanced topics
* Reproducible pipelines with the `targets` package
  * [targets](https://docs.ropensci.org/targets/) - Function-oriented Make-like declarative workflows for R
  * [The {targets} R package user manual](https://books.ropensci.org/targets/)
  * [geotargets](https://docs.ropensci.org/geotargets/index.html) - a `targets` extension for working with geospatial data

</details>


# Version Control with `git` and GitHub

<details>
 
## Core textbooks
* [Chapter 20.1 Git and GitHub in R Packages (2e)](https://r-pkgs.org/software-development-practices.html#sec-sw-dev-practices-git-github)
* [Pro Git](https://git-scm.com/book/en/v2)
* [git for R](https://utdata.github.io/git-for-r/)

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
