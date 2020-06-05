---
author-meta:
- David N. Nicholson
- Jane Roe
bibliography:
- content/manual-references.json
date-meta: '2020-06-05'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta name="citation_title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta property="og:title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta property="twitter:title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta name="dc.date" content="2020-06-05" />

  <meta name="citation_publication_date" content="2020-06-05" />

  <meta name="dc.language" content="en-US" />

  <meta name="citation_language" content="en-US" />

  <meta name="dc.relation.ispartof" content="Manubot" />

  <meta name="dc.publisher" content="Manubot" />

  <meta name="citation_journal_title" content="Manubot" />

  <meta name="citation_technical_report_institution" content="Manubot" />

  <meta name="citation_author" content="David N. Nicholson" />

  <meta name="citation_author_institution" content="Department of Systems Pharmacology and Translational Therapeutics, University of Pennsylvania" />

  <meta name="citation_author_orcid" content="0000-0003-0002-5761" />

  <meta name="twitter:creator" content="@None" />

  <meta name="citation_author" content="Jane Roe" />

  <meta name="citation_author_institution" content="Department of Something, University of Whatever" />

  <meta name="citation_author_institution" content="Department of Whatever, University of Something" />

  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />

  <link rel="canonical" href="https://greenelab.github.io/annorxiver_manuscript/" />

  <meta property="og:url" content="https://greenelab.github.io/annorxiver_manuscript/" />

  <meta property="twitter:url" content="https://greenelab.github.io/annorxiver_manuscript/" />

  <meta name="citation_fulltext_html_url" content="https://greenelab.github.io/annorxiver_manuscript/" />

  <meta name="citation_pdf_url" content="https://greenelab.github.io/annorxiver_manuscript/manuscript.pdf" />

  <link rel="alternate" type="application/pdf" href="https://greenelab.github.io/annorxiver_manuscript/manuscript.pdf" />

  <link rel="alternate" type="text/html" href="https://greenelab.github.io/annorxiver_manuscript/v/8fd66bab1d3b5144aca3b13a0977c48d0d766fae/" />

  <meta name="manubot_html_url_versioned" content="https://greenelab.github.io/annorxiver_manuscript/v/8fd66bab1d3b5144aca3b13a0977c48d0d766fae/" />

  <meta name="manubot_pdf_url_versioned" content="https://greenelab.github.io/annorxiver_manuscript/v/8fd66bab1d3b5144aca3b13a0977c48d0d766fae/manuscript.pdf" />

  <meta property="og:type" content="article" />

  <meta property="twitter:card" content="summary_large_image" />

  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />

  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />

  <meta name="theme-color" content="#ad1457" />

  <!-- end Manubot generated metadata -->'
keywords:
- biorxiv
- preprints
- pubmed central
- natural language processing
- descriptive linguistics
lang: en-US
manubot-clear-requests-cache: false
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
title: Linguistic Analysis of the bioRxiv Preprint Landscape
...






<small><em>
This manuscript
([permalink](https://greenelab.github.io/annorxiver_manuscript/v/8fd66bab1d3b5144aca3b13a0977c48d0d766fae/))
was automatically generated
from [greenelab/annorxiver_manuscript@8fd66ba](https://github.com/greenelab/annorxiver_manuscript/tree/8fd66bab1d3b5144aca3b13a0977c48d0d766fae)
on June 5, 2020.
</em></small>

## Authors



+ **David N. Nicholson**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0003-0002-5761](https://orcid.org/0000-0003-0002-5761)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [danich1](https://github.com/danich1)<br>
  <small>
     Department of Systems Pharmacology and Translational Therapeutics, University of Pennsylvania
     · Funded by GBMF4552; T32 HG00046
  </small>

+ **Jane Roe**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [janeroe](https://github.com/janeroe)<br>
  <small>
     Department of Something, University of Whatever; Department of Whatever, University of Something
  </small>



## Abstract {.page_break_before}




## Introduction
1. What is a preprint
2. Why are preprints important?
3. Mention how preprints are being integrated into scientist’s everyday workflow

1. Talk about biorxiv and discuss how it is one of the repositories that maintains preprints along with citation of others such as arxiv/medrxiv etc.
2. Discuss works that analyze biorxiv from an audience perspective (quantifying tweets etc.)
3. Mention the gap which consists of analysing the language of biorxiv preprints (first to do this)
4. ^ Why is this important? What will this allow for future research projects?
5. Provide list of contributions within this manuscript


## Methods

### Datasets

#### BioRxiv
BioRxiv [@doi:10.1101/833400] is a repository of biological and biomedical research preprints.
We downloaded an xml snapshot of this repository on February 3, 2020 from   bioRxiv's Amazon S3 resource [@https://www.biorxiv.org/tdm] that contained the full text and image content of 98,023 preprints.
Preprints on bioRxiv are versioned, and in our snapshot 26,905 of 98,023 contained more than one version.
When preprints had multiple versions, we used only the latest one. 
Preprints in this snapshot were grouped into one of twenty-nine different categories.
Each preprint was also classified as a new result, confirmatory finding, or contradictory finding.
Some preprints in this snapshot have been withdrawn from bioRxiv.
When a preprint is withdrawn, its content is replaced with the reason for withdrawal.
Because we used the latest version, withdrawn preprints in our analysis contained only statements indicating their removal.

#### PubMed Central
PubMed Central (PMC) [@doi:10.1073/pnas.98.2.381] is a repository that contains free-to-read articles.
PMC contains two types of contributions: closed access articles from research funded by the United States National Institutes of Health (NIH) appearing after an embargo period and articles published under Gold Open Access [@doi:10.1007/s12471-017-1064-2] publishing schemes.
Paper availability within PMC is largely dependent on the journal's participation level [@https://www.ncbi.nlm.nih.gov/pmc/about/submission-methods/].
Individual journals have can fully participate in submitting articles to PMC, selectively participate sending only a few few of papers to PMC, only submit papers according to NIH's public access policy [@https://grants.nih.gov/grants/policy/nihgps/html5/section_8/8.2.2_nih_public_access_policy.htm], or not participate at all.
As of September 2019, PMC had 5,725,819 articles available [@https://www.ncbi.nlm.nih.gov/pmc/about/intro/].
Out of these 5 million articles, about 3 million were open access and available for text processing systems [@doi:10.1093/bioinformatics/btz070;@doi:10.1093/nar/gkz389].
We downloaded a snapshot of this open access subset on January 31, 2020.
This snapshot contains papers such as literature reviews, book reviews, editorials, case reports, research articles and more; however, we used only the research articles.

### Comparing Corpora
We used gensim [@raw:rehurek_lrec] (version 3.8.1) to preprocess the bioRxiv and PubMed Central corpora.
We removed the 337 gensim-provided stopwords.
Throughout our analysis we encountered non-word symbols (e.g., $\pm$), so we refer to words and symbols as tokens to avoid confusion.

Following the cleaning process, we calculated the frequency of every token shared between both corpora.
Because many tokens were unique to one set or the other and observed at low frequency, we used the union of the top 100 most frequent tokens from each corpus to compare them.
We generated a contingency table and calculated the odds ratio for each token.
Furthermore, we also calculated the 95% confidence interval for each odds ratio [@https://www.ncbi.nlm.nih.gov/books/NBK431098/].

### Visualizing the Preprint Landscape

#### Generate Document Representation
1. Describe how word2vec works
2. Talk about training word2vec on entire biorxiv repository
3. Discuss how to generate a document representation using word2vec model

#### Dimensionality Reduction of Document Embeddings
1. Explain how tSNE works (paragraph one)
2. Explain how PCA works  (paragraph two)
3. Discuss how words were mapped onto PC components via cosine similarity
4. ^ Explain cosine similarity

### Recommending Journals/ bioRxiv Audience Analysis
1. This title will update as analysis is completed
2. This section will describe how the above process is conducted


## Results

### Comparing bioRxiv to PubMed Central

#### Global View
1. Create a treemap visualization of top X terms that are different between bioRxiv and PubMed Central (based on odds ratio)

#### Published Preprint Differences
1. Create a treemap visualization of top X terms that are different between Preprint and Published documents (based on odds ratio)

### The bioRxiv Preprint Landscape
1. Provide the tSNE figure of the bioRxiv 
2. Discuss the results of the tSNE figure and highlight that there are category clusters within the figure

### Topic Analysis of Principal Components
1. Provide an example of the word cloud for principal components
2. Show plot of the principal components and the scatterplot
3. Mention that the word clouds can be found at xyz

### Journal Recommendations/Audience Associations
1. Title will change once analysis is finished 
2. Provide key figure for this section and take-home message


## Discussion


## Conclusion


## Acknowledgements


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
