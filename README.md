# README

## ABOUT

This repository contains the code portion of a research project performed as part of a Computational and Statistical Text Analysis course. (CMU 36-662)

The broad research questions were: 
 1. How similar are the rhetorical strategies of politically radical video content made for YouTube from the Left wing and Right wing? 
 2. Does the morally loaded language in left and right wing Youtube videos match the moral arguments expected by the [Moral Foundations Hypothesis](https://moralfoundations.org/) ?
 
## DESCRIPTION

### Data

The underlying data comes from YouTube primarily, using their automatic text transcription which accompanies most videos uploaded to the platform. 
I identified the channels and their political partisanship using recent literature, aggregators, and my own judgement. 
I found the videos using the google API, and scraped the data using [a related repository](https://github.com/follperson/youtube-transcript-scraper) .
The text transcripts were then tagged using [DocuScope](https://www.cmu.edu/dietrich/english/research/docuscope.html) , which is designed for rhetorical analysis.

See examples here: 
* [Cleaned Transcript](/ex/RawTranscript.txt)
* [Docuscope tagged](/ex/DocuscopeTaggedTranscript.txt)

The underlying data is available in the data.7z file, compromising about 36000 video transcrips in tagged and cleaned formats. 
The code also relies on a handful of metadata files, included in the data/docuscope/ and data/youtube/compiled folders, witihin the zipped file.

### Setup

To rerun the analysis:
* clone the repo to your local
* unzip the `data.7z.001, data.7z.002, data.7z.003` using [7zip](https://www.7-zip.org/) in your local repo,
* install any necessary packages as evidenced in the first chunk of the `Partisan Youtube Rhetorical Strategy - Technical Report.rmd` file
* knit the file, or execute the code chunk by chunk. 

### Methods

* Hierarchial Agglomerative Clustering
* K-means clustering
* Multi-Dimensional Analysis (Multi Factor Analysis)
* Keyword analysis 

## ACKNOWLEDGEMENTS & DISCLOSURE

[Dr. David Brown](https://www.cmu.edu/dietrich/english/people/faculty/bios/david-brown.html) for his course and direction, his instrumental helper functions at [/resources/functions](/resources/functions), and his tagging of my transcript data with DocuScope tagging software.

[Contrapoints](https://www.youtube.com/channel/UCNvsIonJdJ5E4EXMa65VYpA) for introducing me to political youtube!

