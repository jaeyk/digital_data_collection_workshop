# Research Workshop on Computational Tools for Digital Data Collection

If you have comments, questions, or suggestions, then [create an issue](https://github.com/jaeyk/digital_data_collection_workshop/issues).

## Description

The focus of this workshop is on digital data collection using R (most cases), Python, and UNIX command-line tools. Three lecture-style sessions will introduce graduate students to advanced techniques in web-scraping, pdf-scraping, and social media scraping. Three seminar-style courses will provide graduate students with the opportunity to receive feedback on strategies for collecting data.

The objective of this workshop is practical: graduate students will develop and execute data collections strategies in each of the three thematic modules, with the final deliverable being three complete and clean datasets. As such, we will expect graduate students involved in the workshop to identify resources---e.g., administrative databases, archival documents, social media accounts---that they wish to scrape.

The emphasis of this course is on data collection, rather than data analysis. However, as the goal of data collection is typically analytical, we will assume a familiarity with conventional approaches to statistical inference in the social sciences.

## Logistics

### Co-instructors

[Jae Yeon Kim](https://jaeyk.github.io/)

jaeyeonkim@berkeley.edu

Nicholas Kuipers

nkuipers@berkeley.edu

### Time and Location

Date: TBD

Location: Zoom

All course materials will be posted on Github at https://github.com/jaeyk/digital_data_collection_workshop, including class notes, code demonstrations, sample data, and assignments.

### Accessibility

This class is committed to creating an environment in which everyone can participate, regardless of background, discipline, or disability. If you have a particular concern, please come to me as soon as possible so that we can make special arrangements.

### Books and Other Resources
There are no official textbooks for this class. Please see [the references](https://github.com/jaeyk/digital_data_collection_workshop/blob/master/B_references.md) (will be updated throughout the semester) for additional references and [the style guides](https://github.com/jaeyk/PS239T/blob/master/style_guides.md) for efficient programming and project management.

### Computer Requirements

The software needed for the course is as follows:

* Access to the UNIX command line (e.g., a Mac laptop, a Bash wrapper on Windows)
* Git
* R and RStudio (latest versions)
* Anaconda and Python 3 (latest versions)

This requires a computer that can handle all this software. Almost any Mac will do the job. Most Windows machines are fine too if they have enough space and memory.

You must have all the software downloaded and installed PRIOR to the first day of class.

See [this guideline](https://github.com/jaeyk/PS239T/blob/master/B_Install.md) for more information on installation.

## Curriculum Outline / Schedule

The schedule is subject to change based on the class's rate of progress.

### Techniques in automating data collection workflow [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jaeyk/digital_data_collection_workshop/master?urlpath=rstudio) [[Notebook](https://rawcdn.githack.com/jaeyk/digital_data_collection_workshop/2012a06f65512da52afa0d970a38e57b31aa8c84/LectureNotes/01_introduction/01_automate_data_collection_workflow.html)]

- September 16, 2020: Automating data collection workflow
    - Instructor: Kim
    - Style: Lecture
    - Description: introduction to the tidyverse; discussion of efficient and reproducible ways to collect and wrangle data
    - R Packages: [dplyr](https://dplyr.tidyverse.org/), [purrr](https://purrr.tidyverse.org/)
    - References:
        - Kim, How to Automate Repeated Things in R ([GitHub](https://github.com/dlab-berkeley/R-functional-programming))
        - Kim, Advanced Wrangling Workshop in R ([GitHub](https://github.com/dlab-berkeley/advanced-data-wrangling-in-R))

### Techniques in social media scraping

- September 23, 2020: Introduction to tweet parsing
    - Lead Instructor: Kim
    - Style: Lecture
    - Description: Introduction to techniques of collecting and parsing social media data with emphasis on Twitter
    - Requirement: Please sign up a [Twitter developer account](https://developer.twitter.com/en/apply-for-access) at least 2-3 days prior to the session.
    - Command-line tool
        - Dehydration: [twarc](https://github.com/DocNow/twarc)
            - [Installation guideline](https://scholarslab.github.io/learn-twarc/05-install-twarc.html) 
    - R packages: 
        - RESTful API: [tweetscores](https://github.com/pablobarbera/twitter_ideology/tree/master/pkg/tweetscores), [twitteR](https://cran.r-project.org/web/packages/twitteR/twitteR.pdf), [rtweet](https://github.com/ropensci/rtweet)
        - Streaming API: [streamR](https://github.com/pablobarbera/streamR)
        - Parsing: [tidyjson](https://cran.r-project.org/web/packages/tidyjson/vignettes/introduction-to-tidyjson.html), [tidytweetjson](https://github.com/jaeyk/tidytweetjson)
    - References:
        - [Benoit](https://www.lse.ac.uk/Methodology/People/Academic-Staff/Kenneth-Benoit/Kenneth-Benoit) and [Tsvetkova](https://www.lse.ac.uk/Methodology/People/Academic-Staff/Milena-Tsvetkova/Milena-Tsvetkova). [LSE MY472 Data for Data Scientists](https://lse-my472.github.io/week10/MY472-week10.pdf)
        - Steinert-Threlkeld, [2020 APSA Short Course Generating Event Data From Social Media](https://github.com/ZacharyST/APSA2020_EventDataFromSocialMedia)
        - Kim, SQL for R Users ([GitHub](https://github.com/dlab-berkeley/sql-for-r-users))
        - Kim, Large-scale Twitter Analysis on COVID-19 and Anti-Asian Climate ([GitHub](https://github.com/jaeyk/covid19antiasian))

- September 30, 2020: Tweet parsing workshop
    - Instructor: Kim + Kuipers
    - Style: Seminar
    - Description: Graduate students provide/receive feedback on tweet parsing data collection strategies

### Techniques in pdf-scraping

- October 7, 2020: PDF-parsing
    - Lead instructor: Kuipers
    - Style: Lecture
    - Description: introduction to techniques of pdf-scraping; where to look for documents; how to know what to pre-process by hand; identifying recurring patterns in text to exploit for data wrangling; parallel processing
    - R Packages: tesseract, magick, zoo, parallel, pdftools
    - References:
        - Mock, [Bear and pdftools](https://themockup.blog/posts/2020-04-03-beer-and-pdftools-a-vignette/)

- October 14, 2020: No workshop -- Indigenous peoples’ day

- October 21, 2020: PDF-parsing workshop
    - Instructor: Kuipers + Kim
    - Style: Seminar
    - Description: Graduate students provide/receive feedback on PDF-parsing data collection strategies

### Techniques in web-scraping

- October 28, 2020: Web-scraping
    - Instructor: Kuipers
    - Style: Lecture
    - Description: introduction to techniques of web-scraping; identifying and exploiting underlying database structures; knowing when to quit
    - R Packages: rvest, jsonlite, zoo, xml, [ralger](https://github.com/feddelegrand7/ralger)
    - Chrome plugin: SelectorGadget
    - References:
        - Terman, 3I: Web Scraping and Data Management in R ([GitHub](https://github.com/rochelleterman/ESS-webscraping))

- November 4, 2020: Web-scraping workshop
    - Instructor: Kuipers + Kim
    - Style: Seminar
    - Description: Graduate students provide/receive feedback on web-scraping data collection strategies
