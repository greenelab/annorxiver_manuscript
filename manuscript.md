---
author-meta:
- David N. Nicholson
- Jane Roe
bibliography:
- content/manual-references.json
date-meta: '2020-05-24'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta name="citation_title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta property="og:title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta property="twitter:title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta name="dc.date" content="2020-05-24" />

  <meta name="citation_publication_date" content="2020-05-24" />

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

  <link rel="alternate" type="text/html" href="https://greenelab.github.io/annorxiver_manuscript/v/28cc3118f87472d30995a33761f91cd6534393bc/" />

  <meta name="manubot_html_url_versioned" content="https://greenelab.github.io/annorxiver_manuscript/v/28cc3118f87472d30995a33761f91cd6534393bc/" />

  <meta name="manubot_pdf_url_versioned" content="https://greenelab.github.io/annorxiver_manuscript/v/28cc3118f87472d30995a33761f91cd6534393bc/manuscript.pdf" />

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
([permalink](https://greenelab.github.io/annorxiver_manuscript/v/28cc3118f87472d30995a33761f91cd6534393bc/))
was automatically generated
from [greenelab/annorxiver_manuscript@28cc311](https://github.com/greenelab/annorxiver_manuscript/tree/28cc3118f87472d30995a33761f91cd6534393bc)
on May 24, 2020.
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

#### bioRxiv
1. Describe how bioRxiv was obtained
2. Describe metadata statistics on bioRxiv (number of preprints, number of preprints with multiple versions)

#### PubMed Central
1. Describe how PubMed central was obtained
2. Describe metadata statistics on PubMed central (number of articles, how many articles were processed

### Comparing Corpora
1. Spacy to process text via - Lemmatization, removal of stop words
2. Describe counting frequencies of each lemma
3. Describe using chi-square test
4. Describe how to calculate the likelihood and log odds ratio

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
