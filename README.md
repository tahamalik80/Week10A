# Assignment 10A — Sentiment Analysis

Author: Taha Malik
Date: 2025-11-02

This repository contains the deliverables for Assignment 10A (Sentiment Analysis), which reproduce the primary example from Robinson & Silge's *Text Mining with R* (Chapter 2) and extend it by (1) applying the workflow to a different corpus (Mark Twain novels from Project Gutenberg), and (2) incorporating an additional sentiment lexicon (Loughran). The R Markdown also demonstrates practical improvements (negation handling and sentence-level sentiment) and includes cached output CSVs to help graders inspect results without re-running heavy downloads.

Primary citation
- Robinson, J. S. and Silge, J. "2 Sentiment analysis with tidy data", Text Mining with R: A Tidy Approach. https://www.tidytextmining.com/sentiment.html

What to look for in the knitted HTML
- Reproduction of textbook examples (Jane Austen).
- Twain corpus analysis (Tom Sawyer & Huckleberry Finn) and discussion.
- Lexicon comparison plots (AFINN, Bing, NRC, and Loughran if available).
- Interpretation paragraphs under each major figure (explaining what the plot means and linking to word-level evidence).
- Quantitative lexicon summary (mean and sd of chunk-level sentiment by lexicon).
- Demonstrations of negation handling (bigrams) and sentence-level sentiment (sentimentr).
- Cached CSVs in `outputs/` for quick verification.

How to reproduce (quick steps)
1. Clone or download this repository.
2. Open `Assignment10A_Sentiment_Analysis_MuahMuahXOXO.Rmd` in RStudio.
3. Ensure you have internet access (required to install packages and download Gutenberg texts).
4. Knit the Rmd to HTML (click the Knit button).
   - The top of the Rmd contains code that installs any missing CRAN packages.
5. After knitting, three CSV files will be created in the `outputs/` folder (they are also included in the repo if you prefer not to run).
6. Publish the knitted HTML to RPubs (RStudio -> Publish -> RPubs) and copy the RPubs URL for submission.

Notes for graders / quick checks
- If package installation fails, run `install.packages()` for the required package(s) and re-knit.
- The `loughran` lexicon is obtained via `get_sentiments("loughran")`. If it's not present, run `install.packages("textdata")` and then try again. The Rmd handles this gracefully and will skip Loughran plots if the lexicon is unavailable; the CSV in `outputs/` indicates whether Loughran results are present.
- The `outputs/` CSVs let you audit numbers without re-downloading texts.
- The Rmd includes `sessionInfo()` output at the end; include that in grading reproducibility checks.

Links: GitHub .Rmd: <[paste URL](https://github.com/tahamalik80/Week10A)>
RPubs: <[paste RPubs URL](https://rpubs.com/tmalik03/WEEK10A)>."

