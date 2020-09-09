---
author-meta:
- David N. Nicholson
- Jane Roe
bibliography:
- content/manual-references.json
date-meta: '2020-09-09'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta name="citation_title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta property="og:title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta property="twitter:title" content="Linguistic Analysis of the bioRxiv Preprint Landscape" />

  <meta name="dc.date" content="2020-09-09" />

  <meta name="citation_publication_date" content="2020-09-09" />

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

  <link rel="alternate" type="text/html" href="https://greenelab.github.io/annorxiver_manuscript/v/fc9f5ff2e9cda3e6c661b3012957c939cbd3bedc/" />

  <meta name="manubot_html_url_versioned" content="https://greenelab.github.io/annorxiver_manuscript/v/fc9f5ff2e9cda3e6c661b3012957c939cbd3bedc/" />

  <meta name="manubot_pdf_url_versioned" content="https://greenelab.github.io/annorxiver_manuscript/v/fc9f5ff2e9cda3e6c661b3012957c939cbd3bedc/manuscript.pdf" />

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
([permalink](https://greenelab.github.io/annorxiver_manuscript/v/fc9f5ff2e9cda3e6c661b3012957c939cbd3bedc/))
was automatically generated
from [greenelab/annorxiver_manuscript@fc9f5ff](https://github.com/greenelab/annorxiver_manuscript/tree/fc9f5ff2e9cda3e6c661b3012957c939cbd3bedc)
on September 9, 2020.
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
We downloaded an xml snapshot of this repository on February 3, 2020 from   bioRxiv's Amazon S3 resource [@url:https://www.biorxiv.org/tdm] that contained the full text and image content of 98,023 preprints.
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
Paper availability within PMC is largely dependent on the journal's participation level [@url:https://www.ncbi.nlm.nih.gov/pmc/about/submission-methods/].
Individual journals have can fully participate in submitting articles to PMC, selectively participate sending only a few few of papers to PMC, only submit papers according to NIH's public access policy [@url:https://grants.nih.gov/grants/policy/nihgps/html5/section_8/8.2.2_nih_public_access_policy.htm], or not participate at all.
As of September 2019, PMC had 5,725,819 articles available [@url:https://www.ncbi.nlm.nih.gov/pmc/about/intro/].
Out of these 5 million articles, about 3 million were open access and available for text processing systems [@doi:10.1093/bioinformatics/btz070;@doi:10.1093/nar/gkz389].
We downloaded a snapshot of this open access subset on January 31, 2020.
This snapshot contains papers such as literature reviews, book reviews, editorials, case reports, research articles and more; however, we used only the research articles.

### Comparing Corpora
We compared bioRxiv against Pubmed Central's Open Access corpus (PMCOA) and the New York Times Annotated corpus (NYTAC) [@raw:sandhaus2008new] to assess the similarities and differences between bioRxiv, PMCOA and NYTAC.
Throughout our analysis we encountered non-word symbols (e.g., $\pm$), so we refer words and symbols as tokens to avoid confusion.
We calculated the following statistics for each corpus: the number of documents, the number of sentences, the total number of tokens, the number of stopwords, the average length of a document, the average length of a sentence, the number of negations, the number of coordinating conjunctions, the number of pronouns and the number of past tense verbs.
Next, we used spaCy's "en_core_web_sm" model [@raw:spacy2] (version 2.2.3) to preprocess all corpora and filtered out 326 spaCy-provided stopwords.  

Following the cleaning process, we calculated the frequency of every token across all corpora.
Because many tokens were unique to one set or the other and observed at low frequency, we used the union of the top 100 most frequent tokens from each corpus to compare them.
We generated a contingency table for each token and calculated the odds ratio from every generated table.
We also calculated the 95% confidence interval for each token's odds ratio [@https://www.ncbi.nlm.nih.gov/books/NBK431098/] and measured corpus similarity by calculating the KL divergence across all three corpora.

### Visualizing the Preprint Landscape

#### Generate Document Representation
We used gensim [@raw:rehurek_lrec] (version 3.8.1) to train a word2vec continuous bag of words (CBOW) [@arxiv:1301.3781] model over the bioRxiv corpus. 
Our neural network architecture had 300 hidden nodes, and we trained this model for 20 epochs.
We set a fixed random seed and otherwise used gensim's default settings.
Following training, we generated a document vector for every article within bioRxiv and PubMed Central.
This document vector is calculated by taking the average of every token present within a given article, ignoring those that were absent from the word2vec model.

#### Dimensionality Reduction of Document Embeddings
We used principal component analysis (PCA) [@doi:10.1111/1467-9868.00196] to project bioRxiv document vectors into a low dimensional space.
We trained this model using scikit-learn's [@raw:scikit-learn] implementation of a randomized solver [@arxiv:0909.4061] with a random seed of 100, output of 50 principal components, and default settings for all other parameters.
For each principal component we calculated its cosine similarity with  all tokens in our word2vec model's vocabulary.
We report the top 100 positive and negative scoring tokens in the form of  word clouds, where the size of each word corresponds to the magnitude of similarity and color represents positive (blue) or negative (orange) association.

### Discovering Unannotated Preprint-Publication Relationships

Automated procedures are in place to link preprints to peer reviewed versions and many journals require authors to update preprints with a link to the published version.
However, automated procedures at _bioRxiv_ are often based on exact matching of certain attributes and authors can forget to establish a link after publication.
For example, authors can change the title between a preprint and published version (e.g., [@doi:10.1101/376665] and [@doi:10.1242/bio.038232]), which prevents _bioRxiv_ from automatically establishing a link.
If the authors do not report the publication to _bioRxiv_, the preprint and the published version are treated as distinct entities despite representing the same underlying research. 
We recognized that the distance in embedding space could reveal preprint to published version links that were missed by existing automated processes.
First, we used CrossRef [@doi:10.1629/uksg.233] to identify bioRxiv preprints that were linked to a corresponding published article.
We filtered out links that contained papers not in PubMed Central's Open Access corpus.
Following the preprocessing step, we calculated the distribution of known preprint to published distances by taking the Euclidean distance between the preprint's embedding coordinates and the coordinates of the published version.
We also calculated a background distribution, which consisted of the distance between each preprint with an annotated publication and a randomly selected article from the same journal the published version.
Next, we calculated distances between preprints without a published version link with PubMed Central articles that weren't matched with a corresponding preprint.
We filtered any potential links with distances that were greater than the minimum value of the background distribution to reduce the curation burden.
Lastly, we binned the remaining pairs based on percentiles from the annotated pairs at the [0,25th percentile), [25th percentile, 50th percentile), [50th percentile, 75th percentile), and [75th percentile, minimum background distance).
We randomly sampled 50 articles from each bin for manual annotation.
We shuffled these four sets to produce a list of 200 potential preprint-published pairs with a randomized order.
We supplied these candidates to two scientists to manually determine if each link between a preprint and a putative matched version was correct or incorrect.
After the curation process we encountered eight mismatches.
These mismatches were supplied to a third scientist, who carefully reviewed each case and made a final determination.
Lastly, we used this curated set to evaluate the extent to which distance in the embedding space revealed true but unannotated links between preprints and their published verisons.

### Journal Recommendation

We aimed to predict the journal a paper would eventually be published in based on its embedding representation.
We illustrate our recommendations as a short list along with a network visualization available at [https://greenelab.github.io/annorxiver-journal-recommender/](https://greenelab.github.io/annorxiver-journal-recommender/).
Since we sought to examine if embeddings were related to publication venue, we used a simple k-nearest neighbors approach with Euclidean distance to recommend journals.

First, we filtered all journals that had fewer than 100 papers in the PMC dataset.
A subset of our PMC corpus was directly linked to papers in bioRxiv as they had been published as open access articles.
We held out this subset and treated it as our gold standard test set.
We used the remainder of the PMC corpus for training and initial evaluation via cross validation.
We considered a list of ten journal suggestions to be an appropriate number and we considered a prediction to be a true positive if the correct journal appeared within the ten closest neighbors of the query article.

Certain journals publish articles in a focused topic area, while others publish articles that cover many topics.
Likewise, some journals have a publication rate of at most hundreds of papers per year while others publish at a rate of at least ten-thousand papers per year.
Accounting for these characteristics, we designed two approaches for recommending journals.

The first approach is based on individual paper proximity, which enabled us to provide an example of the specific article or articles that led to the prediction.
Conversely, predictions using this technique could be biased due to the overrepresentation of general topic journals.
We call this approach the paper-based classifier.
This classifier takes a query article that has been projected onto the embedding space trained on bioRxiv preprints as input and reports the journals of the top ten closest papers.
The number of journals returned via this method could be less than ten as multiple papers in close proximity to query article may belong to the same journal. 

The second approach is based on close proximity to a journal's centroid.
This technique provides recommendations that are more focused on domain-specific publication venues.
We call this approach the journal-based classifier.
This classifier was trained by computing journal centroids via taking the average embedding of all papers published in each journal.
Following the centroid calculation, this classifier takes a query article projected onto the same embedding space as above for input and reports the top ten nearest journals centroids.
Both the paper-based classifier and the journal-based classifier were optimized via 10-fold cross validation.
We evaluated performance of both classifiers on our gold standard test set of published preprints.

We used SAUCIE [@doi:10.1101/2020.03.04.975177] to train a model that uses the latent space of a neural network to learn an embedding suitable for visualization.
This model enabled us to visualized the PMC corpus and to efficiently embed new papers and preprints with the space.
We trained this model using a learning rate of 0.001, lambda_b of 0, lambda_c of 0.001, and lambda_d of 0.001 for 2000 iterations.
We used the fully trained model to project user-requested _bioRxiv_ preprints onto the generated landscape to enable users to see where their preprint falls along the landscape.


## Results

### Comparing bioRxiv to PubMed Central

#### bioRxiv Repository

![
Neuroscience and bioinformatics are the two most common topics for preprints on bioRxiv.
This bar chart depicts the number of preprints that fall into each author-selected topic area.
](https://raw.githubusercontent.com/greenelab/annorxiver/35d3ea0de3c9c78e3c524736bbaada00928c88fb/biorxiv/exploratory_data_analysis/output/figures/preprint_category.png){#fig:biorxiv_categories}

![
Most of bioRxiv's preprints report new research findings.
This bar chart depicts the number of articles categorized based on author-selected article types.
](https://raw.githubusercontent.com/greenelab/annorxiver/94874e0f1e35bd667bf3b7c3dc6416068779444f/biorxiv/exploratory_data_analysis/output/figures/preprint_headings.png){#fig:biorxiv_headings}

Each preprint on bioRxiv has an author-selected topic area, and the predominant area in past reports has been neuroscience [@doi:10.7554/eLife.45133].
Our analysis of the full text release of bioRxiv confirms this previous finding (Figure {@fig:biorxiv_categories}).
The author-selected topic area abundances that we found in the full text largely matched previous studies [@doi:10.7554/eLife.45133; @doi:10.1001/jama.2017.21168].
One exception was microbiology, which has a larger share of preprints than in a previous report from 2018 [@doi:10.7554/eLife.45133] (Figure {@fig:biorxiv_categories}).
Authors also select from three article types when they upload their preprints.
We found that most preprints are categorized as new results (Figure {@fig:biorxiv_headings}), which is consistent with previous findings [@doi:10.1001/jama.2017.21168].

#### Global Comparison of bioRxiv and PubMed Central 

![
BioRxiv is more focused on biological discoveries rather than disease treatments and clinical trials.
The plot on the left (A) is a point range plot of the odds ratio with respect to bioRxiv.
Values greater than one indicate a high association with bioRxiv whereas values less than one indicate high association with PubMed Central.
The dotted line provides a breaking point between both categories.
The plot on the right (B) is a bar chart of token frequency appearing in bioRxiv and PMC respectively.
](https://raw.githubusercontent.com/danich1/annorxiver/f5d6c2d04e2fef0d38eaee77ef6c2a0b19ef6358/biorxiv/corpora_comparison/output/figures/biorxiv_vs_pubmed_central.png){#fig:biorxiv_pmc_global_comparison}

The linguistic style of the bioRxiv corpus differs from the PMC corpus.
We compared preprints in bioRxiv with published manuscripts in PMC.
We found that tokens such as "neuron", "genome", "RNA" and "network" had a high odds ratio, indicating enrichment in bioRxiv (Figure {@fig:biorxiv_pmc_global_comparison}).
Likewise, we found tokens such as "patient", "health", $\pm$, and "ml" to have a low odds ratio, indicating enrichment in PMC (Figure {@fig:biorxiv_pmc_global_comparison}).
This separation of tokens suggests a prevalence of articles focused on clinical trials and patient research within PMC compared to bioRxiv.
Furthermore, bioRxiv has a predominance of neuroscience and bioinformatic topics.
In regard to writing, citation styles diversify from the familiar "et al." form as preprints transition through the publication process.
Additionally, published articles have an increase of typesetting ($\pm$) and measurement symbols ("ml", "age") compared to preprints. 

#### Published Preprint Differences

![
Top scoring tokens for preprints are focused on figure citations whereas their published versions are more focused on data availability.
The plot on the left (A) is a point range plot of the odds ratio with respect to preprints.
Values greater than one indicate a high association with preprints while values less than one indicate a high association with published articles.
The dotted line provides a breaking point between both categories.
The plot on the right (B) is a barchart of token frequency appearing in preprints and published versions of preprints respectively.
](https://raw.githubusercontent.com/danich1/annorxiver/f5d6c2d04e2fef0d38eaee77ef6c2a0b19ef6358/biorxiv/corpora_comparison/output/figures/preprint_published_comparison.png){#fig:biorxiv_pmc_pre_published_comp}

A preprint's linguistic style can change once a preprint has undergone the revision process prior to being published.
We quantified this linguistic difference by calculating the odds ratio of tokens appearing in the union in bioRxiv preprints and their published counterparts within PMC.
Tokens with an odds ratio greater than one are mainly centered on paper/figure references and research specific terms (Figure {@fig:biorxiv_pmc_pre_published_comp}).
Tokens with an odds ratio of less than one are focused on data availability, and research measurements such as number of cases and controls or significance testing (Figure {@fig:biorxiv_pmc_pre_published_comp}).

### Topic Analysis of bioRxiv's Principal Components

![
The top two principal components (PCs) appear to capture the concepts of molecular biology vs quantitative biology (PC1) and neuroscience vs bioinformatics (PC2).
The word clouds (A, C) depict the cosine similarity score between tokens and the first two PCs.
Tokens in orange are most similar to a PC's positive direction while tokens in blue are most similar to a PC's negative direction.
The size of each token indicates the magnitude of the similarity score.
The scatter plot at the top right (B) is a visualization of documents being plotted along the PC directions.
Article categories were hand-picked based on the concepts captured by each PC.
](https://raw.githubusercontent.com/greenelab/annorxiver/35d3ea0de3c9c78e3c524736bbaada00928c88fb/biorxiv/pca_association_experiment/output/pca_plots/figures/pca01_v_pca02_figure.png){#fig:pca_word_cloud_plot}

![
Preprint categories have a diverse spread of quantitative and molecular biology results.
This is box plot shows preprints in each article category projected along the PC1 direction.
Negative values indicate molecular biology concepts, while positive values indicate quantitative biology concepts.
](https://raw.githubusercontent.com/danich1/annorxiver/4e0c90c590dd7958dc424a1b4fefcecccb3c28ad/biorxiv/pca_association_experiment/output/pca_plots/figures/category_box_plot_pc1.svg){#fig:pca1_pointplot}

![
The second PC groups neuroscience related preprint categories and bioinformatics related preprint categories together.
This is box plot shows preprints in each article category projected along the PC2 direction.
Negative values indicate neuroscience concepts, while positive values indicate bioinformatic concepts.
](https://raw.githubusercontent.com/danich1/annorxiver/4e0c90c590dd7958dc424a1b4fefcecccb3c28ad/biorxiv/pca_association_experiment/output/pca_plots/figures/category_box_plot_pc2.svg){#fig:pca2_pointplot}

| Title [citation]                                                                                                                                                  | PC_1              | License      | Figure Link |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|--------------|------|
| Conditional Robust Calibration (CRC): a new computational Bayesian methodology for model parameters estimation and identifiability analysis [@doi:10.1101/197400] | 4.700554908074704 | None         | https://www.biorxiv.org/content/biorxiv/early/2017/10/02/197400/F1.large.jpg |
| Machine learning of stochastic gene network phenotypes [@doi:10.1101/825943]                                                                                      | 4.410660604449826 | CC-BY-NC-ND  | https://www.biorxiv.org/content/biorxiv/early/2019/10/31/825943/F5.large.jpg |
| Notions of similarity for computational biology models [@doi:10.1101/044818]                                                                                      | 4.355295926618207 | CC-BY-NC-ND  | https://www.biorxiv.org/content/biorxiv/early/2016/03/21/044818/F1.large.jpg |
| GpABC: a Julia package for approximate Bayesian computation with Gaussian process emulation [@doi:10.1101/769299]                                                 | 4.351517618262304 | CC-BY-NC-ND  | https://www.biorxiv.org/content/biorxiv/early/2019/09/18/769299/F1.large.jpg |
| SBpipe: a collection of pipelines for automating repetitive simulation and analysis tasks [@doi:10.1101/107250]                                                   | 4.321847854182741 |  CC-BY-NC-ND | https://www.biorxiv.org/content/biorxiv/early/2017/02/09/107250/F1.large.jpg |
| | | | | |
| Spatiotemporal proteomics uncovers cathepsin-dependent host cell death during bacterial infection [@doi:10.1101/455048]                                           | -4.263964235099807 |  CC-BY-ND   | https://www.biorxiv.org/content/biorxiv/early/2018/11/07/455048/F1.large.jpg |
| Systems analysis by mass cytometry identifies susceptibility of latent HIV-infected T cells to targeting of p38 and mTOR pathways [@doi:10.1101/371922]           | -4.279016673409032 | CC-BY-NC-ND | https://www.biorxiv.org/content/biorxiv/early/2018/07/19/371922/F1.large.jpg |
| NADPH consumption by L-cystine reduction creates a metabolic vulnerability upon glucose deprivation [@doi:10.1101/733162]                                         | -4.592209988884236 | None        | https://www.biorxiv.org/content/biorxiv/early/2019/08/13/733162/F1.large.jpg |
| Inhibition of Bruton’s tyrosine kinase reduces NF-kB and NLRP3 inflammasome activity preventing insulin resistance and microvascular disease [@doi:10.1101/745943] | -4.736613689905791 | None        | https://www.biorxiv.org/content/biorxiv/early/2019/08/28/745943/F1.large.jpg |
| AKT but not MYC promotes reactive oxygen species-mediated cell death in oxidative culture [@doi:10.1101/754572]                                                   | -4.826793742506695 | None        | https://www.biorxiv.org/content/biorxiv/early/2019/09/01/754572/F1.large.jpg |

Table: Top five and bottom five systems biology preprints projected onto the PC1 direction. These preprints contain quantitative and molecular biology concepts respectively. {#tbl:five_pc1_table}

We explored the primary differences between the full text of bioRxiv preprints by performing principal components analysis on generated document embeddings.
We visualized the correspondence between tokens and the loadings for each principal component (Figure {@fig:pca_word_cloud_plot)A,C).
We also visualized documents projected on selected principal components (Figure {@fig:pca_word_cloud_plot)B).
The first principal component separates bioRxiv preprints that encompass molecular biology results with preprints that contain quantitative biology results (Figure {@fig:pca_word_cloud_plot)C).
This highlights the bisection of biomedical research where majority of results can be categorized under the molecular biology category or the quantitative biology category.
Furthermore, this bisecting trend is evident across individual preprint categories as most categories lie on either side of the first principal component (Figure {@fig:pca1_pointplot}).
We also provide example preprints from the systems biology category to reinforce this concept (Table {@tbl:five_pc1_table}).
 
The second principal component represents the concept of neuroscience vs bioinformatics (Figure {@fig:pca_word_cloud_plot)A).
This principal component suggests that the bulk of preprints within bioRxiv are largely focused around neuroscience and bioinformatic concepts.
This split is evident in Figure {@fig:pca2_pointplot} as enriched categories along this principal component are quite related to neuroscience (negative end) or bioinformatics (positive end).
As with the first principal component we provide example preprints from the systems biology category to reinforce this concept (Supplemental Table {@tbl:five_pc2_table}). 
More principal component word clouds can be found on our journal recommender website ([greenelab.github.io/annorxiver-journal-recommender](https://greenelab.github.io/annorxiver-journal-recommender/)) and within our online repository (see Data Availability).

### Journal Recommendations/Audience Associations
1. Title will change once analysis is finished 
2. Provide key figure for this section and take-home message


## Discussion


## Conclusion


## Acknowledgements


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>


## Supplemental Tables

| Title [citation]                                                                                                                                                                                           | PC_2               | License      | Figure Link |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------|--------------|-----|
| Pangenome Analysis of Enterobacteria Reveals Richness of Secondary Metabolite Gene Clusters and their Associated Gene Sets [@doi:10.1101/781328]                                                           | 3.5865702659438883 |  CC-BY-ND    | https://www.biorxiv.org/content/biorxiv/early/2019/09/25/781328/F1.large.jpg |
| QTG-Finder: a machine-learning based algorithm to prioritize causal genes of quantitative trait loci [@doi:10.1101/484204]                                                                                 | 3.470388383023157  | None         | https://www.biorxiv.org/content/biorxiv/early/2019/04/29/484204/F1.large.jpg |
| Identification of candidate genes underlying nodulation-specific phenotypes in Medicago truncotula through integration of genome-wide association studies and co-expression networks [@doi:10.1101/392779] | 3.3814906334073953 |  CC-BY-NC-ND | https://www.biorxiv.org/content/biorxiv/early/2018/08/16/392779/F1.large.jpg |
| Raw sequence to target gene prediction: An integrated inference pipeline for ChIP-seq and RNA-seq datasets [@doi:10.1101/220152]                                                                           | 3.3632576028389742 | None         | https://www.biorxiv.org/content/biorxiv/early/2017/11/16/220152/F3.large.jpg |
| The y-ome defines the thirty-four percent of Escherichia coli genes that lack experimental evidence of function [@doi:10.1101/328591]                                                                      | 3.28742786641417   | CC-BY        | https://www.biorxiv.org/content/biorxiv/early/2018/12/03/328591/F1.large.jpg |
| | | | | |
| The effects of time-varying temperature on delays in genetic networks [@doi:10.1101/019687]                                                                                                    | -2.7047102478958056 | None          | https://www.biorxiv.org/content/biorxiv/early/2015/09/24/019687/F1.large.jpg |
| An analog to digital converter creates nuclear localization pulses in yeast calcium signaling [@doi:10.1101/357939]                                                                            | -2.775745000260895  | None          | https://www.biorxiv.org/content/biorxiv/early/2018/06/28/357939/F1.large.jpg |
| Nicotinic modulation of hierarchal inhibitory control over prefrontal cortex resting state dynamics: modeling of genetic modification and schizophreniarelated pathology [@doi:10.1101/301051] | -3.047342382798414  | None          | https://www.biorxiv.org/content/biorxiv/early/2018/04/13/301051/F1.large.jpg |
| Electrical propagation of vasodilatory signals in capillary networks [@doi:10.1101/840280]                                                                                                     | -3.107715578793087  |  CC-BY-NC-ND  | https://www.biorxiv.org/content/biorxiv/early/2019/11/13/840280/F1.large.jpg |
| Dendritic spine geometry and spine apparatus organization govern the spatiotemporal dynamics of calcium [@doi:10.1101/386367]                                                                  | -3.21533499072831   |  CC-BY-NC-ND  | https://www.biorxiv.org/content/biorxiv/early/2019/05/29/386367/F1.large.jpg|

Table: Top five and bottom five systems biology preprints projected onto the PC2 direction. These preprints contain bioinformatis and neuroscience concepts respectively. {#tbl:five_pc2_table}
