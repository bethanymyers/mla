## What we talk about when we talk about medical librarianship: an analysis of Medical Library Association annual meeting abstracts, 2001-2019

This repository contains code and files to analyze the annual meeting abstracts of the Medical Library Association. The abstracts themselves were taken from the [MLA website](https://www.mlanet.org/page/past-and-future-meetings), converted, and can now be browsed/downloaded in CSV format [here](http://bit.ly/mlameetings).

### Description of files:
- `MLA descriptive` : Jupyter notebook containing basic descriptive code (counts of abstracts, author names, etc)
- `MLA LDA` : Jupyter notebook containing the topic modeling code
- `mla.csv` : MLA meeting abstracts 2001-2019
- `JMLA.csv` : number of JMLA articles to compare with the counts of MLA meeting abstracts (used in the `MLA descriptive` notebook)
- `normalized author list.csv` : contains disambiguated author names that result from running the disabled code block in the `MLA descriptive` notebook. This disabled code block uses fuzzy matching to disambiguate names and takes forever to run, so `normalized author list.csv` is its saved output.
`dict.txt` : the LDA dictionary. LDA will give different results every time, so reusing the same dictionary aids reproducibility.
`model.txt` : the LDA model. LDA will give different results every time, so here is the model I used for my analysis.
- `mla_topics.html` : a standalone version of the pyLDA visualization of the topic model from the `MLA LDA` notebook. You can view it [online](https://bethanymyers.github.io/mla/mla_topics.html)
`mla_authors_by_state.html` : an interactive version of the U.S. map from the `MLA descriptive` notebook.
