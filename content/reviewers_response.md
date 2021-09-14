# Response to Reviewers

## Reviewer #1

> [identifies himself as Ross Mounce]
> 
> This manuscript 'Linguistic Analysis of the bioRxiv Preprint Landscape' presents an analysis of bioRxiv fulltexts and metadata, relative to journal-published versions of the same preprints (n= 17,952 pairs), and the New York Times Annotated Corpus.
> 
> It's an interesting manuscript worthy of publication in PLOS Biology after a few relatively minor revisions.
> 
> I have left many comments directly on the manuscript via the dedicated manuscript website, using public Hypothes.is annotations: https://greenelab.github.io/annorxiver_manuscript/
> 
> I incorporate some but not all of these comments into this formal review supplied to the journal (PLOS Biology) who invited me to review this manuscript.
> 
> Unsurprisingly, biorxiv preprints and journal-published versions of biorxiv preprints are found to be linguistically different to the New York Times Annotated Corpus e.g. in average document length and to a lesser degree in average sentence length, and % in passive voice.
> 
> Luckily there are plenty more actually interesting results reported in this manuscript, not least that of 23,271 preprint-published pairs, 17,952 of those pairs (>77%) had a published version present within the PMCOA corpus.  I don't think the authors quite realise the significance of this result. 77% is a very very high rate of open access. It could do with being discussed more within the manuscript e.g. relative to the overall (lower) rate of open access of _all_ biomedical and life science research articles. What does this signify about preprint authors / 'preprinters'? 
> 
> I can think of a couple of hypotheses:
> 
>  a) preprinters are perhaps more likely to have grant-funded research subject to an open access policy
> 
> b) perhaps preprinters are more publishing 'savvy' and want to achieve more impact/citations and thus strive harder to ensure that the eventual journal-published version of their work is open access (reflected in being in PMCOA).

**We appreciate your positive viewpoint on our manuscript.
The increasing amount of open access articles is an interesting point.
We have updated our discussion to emphasize this point.**
 
> If it were my choice I would cut the entire subsection 'Document embeddings derived from bioRxiv reveal fields and subfields'. It is already known that document embeddings can reveal fields and subfields. Being 'preprints' or 'biorxiv preprints' rather than say published journal articles won't change that. I found this section very uninteresting and extremely un-novel. It is descriptive and accurate, but in the context of an already long manuscript, I feel it is unnecessary.

**We decided that this analysis is necessary for our manuscript.
However, we did move this section into our supplement.**

> Aside from the manuscript, I have some brief comments on the actual web application.
> 
> I tried some palaeontology preprints (it's a field i'm very familiar with). The results were rather mixed.
> e.g. for https://greenelab.github.io/preprint-similarity-search/?doi=10.1101/2020.12.10.406678 ("The first dinosaur egg remains a mystery"), the most similar paper recommendations were excellent. However, the most similar journals suggested were surprisingly poor - many of these could obviously at a glance never publish this preprint (dinosaurs are not plants!) e.g. American Journal of Botany, World Archaeology, Journal of Phycology, The Holocene, Botanical Journal of the Linnean Society. Linnean Society of London
> 
> But I realise that PMCOA isn't exactly great training date for interpreting palaeontology articles -- fringe content from PMC's perspective(?)

**Thank you for pointing this fact out.
We agree that these results highlight a subtle limitation when using PMCOA to train our classifiers.
We would like to point out that our resourse has an auto-updater that monthly incorporates new papers posted to PMCOA.
Overtime this problem could be remedied when PMC posts more published articles related to this area.**
 
> Specific comments:
> 
> 1.) https://hypothes.is/a/1ODs5NLbEeuhnEPjCpUFpA
> 
>I think this needs to be made more specific as [25] analysed a few different things.
>
>Your statement here is true with respect to their analysis of abstract text "Over 50% of abstracts had changes that minorly altered, strengthened, or softened the main conclusions"
>
>BUT
>
>it is not true with respect to the panels and tables analysis in [25]:
>
>"over 70% of 162 published preprints were classified with “no change” or superficial rearrangements to panels and 163 tables, confirming the previous conclusion"
>
>thus perhaps you should consider writing something like:
>
>an analysis of preprints posted at the beginning of 2020 revealed that over 50% underwent minor changes in the abstract text as they were published, but over 70% had 'no change' or only superficial rearrangements to panels and tables [25].

**We thank you for the suggested change and have incorporated the following change within our revised manuscript.**

```diff
- Preprint repositories by definition do not perform in-depth peer review, which can result in posted preprints containing inconsistent results or conclusions [@doi:10.12688/f1000research.19619.2; @doi:10.1007/s10393-018-1352-3; @doi:10.1038/530265a; @doi:10.1016/j.bpj.2016.06.035]; however, an analysis of preprints posted at the beginning of 2020 revealed that most underwent minor changes as they were published [@doi:10.1101/2021.02.20.432090].

+ Preprint repositories by definition do not perform in-depth peer review, which can result in posted preprints containing inconsistent results or conclusions [@doi:10.12688/f1000research.19619.2; @doi:10.1007/s10393-018-1352-3; @doi:10.1038/530265a; @doi:10.1016/j.bpj.2016.06.035]; however, an analysis of preprints posted at the beginning of 2020 revealed that over 50% underwent minor changes in the abstract text as they were published, but over 70% did not change or only had simple rearrangements to panels and tables [@doi:10.1101/2021.02.20.432090].
```

> 2.) https://hypothes.is/a/djNirNLcEeu2YxNM5WBxvA
> 
>but to clarify, you did remove these from the analysis, right? It would just be good to clarify that. They are easy to identify and should just be removed. I can't see how they would add anything but noise to this analysis. What is the total number of preprints after withdrawn preprints are removed from the sample?
 
**No.
We kept these withdrawn preprints within our analysis as the amount wasn't high enough to significantly affect our results.**

> 3.) https://hypothes.is/a/bmdkpNLeEeuZ0k8oLqyeWQ
> 
>actually, there need not necessarily be an embargo period. Many publishers now offer a zero-day embargo so that the author accepted manuscript can be deposited either at acceptance (before even journal publication!) or on the day of journal publication. Even if the journal normally tries to embargo the work, you can see some full text author manuscripts become immediately available well before the journal would normally permit them 'out' thanks to the Plan S Rights Retention Strategy e.g. this one here: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7610590/
>
>So what you should really say here is that full text works appear in PMC as either accepted author manuscripts (green open access) or via open access publishing at the journal (gold open access).
>
>BTW, I resent calling it a 'closed access' [article?] if the accepted manuscript is fully freely available -- that would seem to give undue primacy to the journal published version. It's an article with different versions - one freely accessible at a repository e.g. PMC, without publisher branding and another behind a paywall at the publisher website with publisher branding

**We agree that 'closed access' may not be appropriate for this description.
We have have changed this section in our manuscript.**

```diff
- PMC articles can be closed access ones from research funded by the NIH appearing after an embargo period or be published under Gold Open Access [@doi:10.1007/s12471-017-1064-2] publishing schemes.

+ Articles appear in PMC as either accepted author manuscripts (Green Open Access) or via open access publishing at the journal (Gold Open Access [@doi:10.1007/s12471-017-1064-2]).
```

> 4.) https://hypothes.is/a/-v_PbtLeEeu8Rw8afgzT5g
> 
> presuming a journal allows individual articles to be published with a CC BY licence under a so-called 'hybrid-OA' option, can a journal really NOT participate for those CC BY licenced articles? If biomedically relevant and CC BY licensed surely PMC takes that content at the article level and thus its debatable as to whether journals really have the power to actually 100% not participate.

**We have updated our manuscript to take this point into account.**

```diff
- Individual journals have the option to fully participate in submitting articles to PMC, selectively participate sending only a few papers to PMC, only submit papers according to NIH's public access policy [@url:https://grants.nih.gov/grants/policy/nihgps/html5/section_8/8.2.2_nih_public_access_policy.htm], or not participate at all.

+ Individual journals have the option to fully participate in submitting articles to PMC, selectively participate sending only a few papers to PMC, only submit papers according to NIH's public access policy [@url:https://grants.nih.gov/grants/policy/nihgps/html5/section_8/8.2.2_nih_public_access_policy.htm], or not participate at all; however, individual articles published with the CC BY license may be incorporated.
```

> 5.) https://hypothes.is/a/vekhYNLfEeuxGm9i6MkLqw
> it's a real pity you chose not to compare preprints to author manuscripts. As your results demonstrated, lots of the word changes were just journal-style related e.g. "figure" -> "fig." . An analysis of just preprints matched to author manuscripts would get more closely and cleanly to what the textual difference between pre-peer-review and post-peer-review (without minor stylistic changes).

**We recognize that author manuscripts have the potential to remove some of the journal-related stylistic changes revealed in our token analysis.
However, we leave this potential of this analysis for future endeavors.**

> 6.) https://hypothes.is/a/YkqPKNLgEeucPGc1_W-jzA
> 
> minor typo: tagging surely

**Thank you for pointing this out.
We updated text to fix this typo.**

```diff

- This collection contains over 1.8 million articles where 1.5 million of those articles have undergone manual entity tagged by library scientists [@sandhaus2008new].

+This collection contains over 1.8 million articles where 1.5 million of those articles have undergone manual entity tagging by library scientists [@sandhaus2008new].
```

> 7.) https://hypothes.is/a/Bsv68tLkEeugHEfCZMUGag
> From the perspective of a person (me!) interested in open access to ('final') peer-reviewed research outputs this is a super interesting result in itself, which should perhaps be remarked upon more in this manuscript.
>
>It implies that over 77% (17,952/23,271) of biomedical preprints that are detectably linked to a journal published paper, that subsequent journal published paper became open access in the PMCOA corpus (regardless of specific means/route). That's great news. The subset of works from biomedical researchers that do preprinting have a much higher level of open access (to the eventual journal published version) than biomedical research overall (including works that don't have a preprint version)
>
>See figure 3a from 'Open access levels: a quantitative exploration using Web of Science and oaDOI data' by Bosman and Kramer for a comparator looking at OA levels in biomedical and life science papers https://peerj.com/preprints/3520.pdf even in the 'best' OA performing subfield (Cell Biology) it doesnt reach 70%. 30% to 50% is more typical albeit looking at 2016 publications.
>
>Put another way, we only 'lose' 23% of biomedical preprinted research to paywalled journals that do not allow a copy of the work to be made full text available in the PMCOA corpus, in reasonable time**. And in those cases we still have access to the preprint
>
>** with no doubt many other caveats such as cases where the author could do it without help from the journal, but does not for some unknown reason

**We appreciate you point out this interesting fact and we have updated our discussion accordingly.**

```diff
+ Over 77% of bioRxiv preprints that were published ended up within Pubmed Central's Open Access Corpus (PMCOA) which is a significant improvement compared to the earlier years [@doi:10.7287/peerj.preprints.3520v1].
+ This highlights a beneficial shift towards more preprint authors publishing their work in an open access format.
```

> 8.) https://hypothes.is/a/aWmt3tLlEeuh3M-Ku8ThvQ
> 
> To be clear 326 stopwords is the default setting?
>
>Interestingly 'ca' is one of those 326 stopwords. I would have thought that one might actually be significant in a life sciences context e.g. calcium channels "Ca2+"

**Yes, 326 stopwords are the default setting.** 


> 9.) https://hypothes.is/a/dkIurtLmEeuqkU-qTN4dtg
> 
> I'm sure you've got this in the github, but just to make the manuscript more readily understandable without digging around in github, do you think you could provide as a supplementary file a list of those 100 most frequently occurring tokens, so that people can get a better feel for what the data is here?

**We have added a supplementary file that provides a listing of 100 tokens for our corpora KL analysis.**

> 10.) https://hypothes.is/a/-2AU8tLmEeu6swvY4jN5Mw
> 
> hmmm… not a problem of this manuscript, but that's really not good enough from bioRxiv is it? Change one word of a long and complex title and suddenly 'oh, we can't do it'. A comment to suggest that bioRxiv could do better would be fun, no(?) i.e. look at author names AND title and if both are similar enough, then do auto-linking.
> 
> oh okay, you did actually do that. Nice :)

**We are glad that you like our document matching solution.**

> 11.) https://hypothes.is/a/dhGbgNLnEeuYkkfUNqKwgA
> 
> I don't suppose you could possibly be precise about this rather than just 'a limited number'? Is it 5, 50, or 500?

**We agree that this line is a bit vague and have updated our text to be more explicit.**

```diff

- There were a limited number of cases in which authors appeared to post preprints after the publication date, which results in preprints receiving a negative time difference, as previously reported [@url:https://medium.com/@OmnesRes/the-biorxiv-wall-of-shame-aa3d9cfc4cd7]

+ We encountered 123 cases where the preprint posting date was subsequent to the publication date, resulting in a negative time difference, as previously reported [@url:https://medium.com/@OmnesRes/the-biorxiv-wall-of-shame-aa3d9cfc4cd7].
```

> 12.) https://hypothes.is/a/DzrzGtLtEeuJlcdOlUfUBA
> 
> I'm surprised to see no citation given to JANE: https://jane.biosemantics.org/
>
>https://academic.oup.com/bioinformatics/article/24/5/727/202224
>
>reviewed in https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6300233/
>
>The 'find journals' functionality of JANE appears somewhat similar to the discovering similar journals functionality here.

**Thank you for pointing this citation out. 
We have incorporated it into our manuscript.**

```diff
- We developed a web application that places any bioRxiv or medRxiv preprint into the overall document landscape and identifies similar papers and journals.

+ We developed a web application that places any bioRxiv or medRxiv preprint into the overall document landscape and identifies topically similar papers and journals (similar to [@doi:10.5195/jmla.2019.598]).
```

> 13.) https://hypothes.is/a/eJ7-DtLpEeuh0A8OL8WAWw
> 
> This is the kind of journal-faff difference that I hypothesise would not be visible or less visible if one did an analysis of preprints vs author manuscripts.
>
>There is change but is change from figure to 'fig.' to suit journal style actually helpful/valuable? In my opinion it is not!

**We recognize the limitation of our design choice and have mentioned using accepted author manuscripts as an alternative for future analyses.**

> 14.) https://hypothes.is/a/-ixA_NLqEeuv6YviR-lI0A
> 
> I would cut this entire subsection from the manuscript to make it shorter (or relegate it to a supplementary section).
>
>Don't we already know that if one uses full texts we can determine the subfield of the paper? It's not that interesting in my opinion and not relevant to the main hypotheses of the paper -- comparing between preprints and the journal published version.

**We believe this section is needed when performing a descriptive analysis on the bioRxiv corpus; however, we moved this section to the supplement.**

> 15.) https://hypothes.is/a/V2wj3NLqEeuZ9idQ44yS4Q
> 
> adjusting for recency? i.e. not sampling 2019 preprints? in figure C the line indicates (if I'm interpreting correctly) that overall only 46.55% are published but that's because it includes very recent preprints that haven't had time to be journal published yet. Just be explicit that you are adjusting for recency (i.e. excluding 2019 and newer preprints) when you say that most preprints are eventually published.

**We included all preprints (from 2013 to 2019 and newer) posted onto biorxiv when calculating the overall proportion of preprints published.**

> 16.) https://hypothes.is/a/N8cKltLrEeuZ-iPc5lrP5g
> 
> text changes relative to the journal published version? You might want to make that more explicit. Text changes alone is not adequately specific in my opinion.

**We agree that text changes was a bit vauge and have updated the title accordingly.**

```diff
- Preprints with more versions or more text changes took longer to publish

+ Preprints with more versions or more text changes relative to their published counterpart took longer to publish
```

> 17.) https://hypothes.is/a/z4r5ztLgEeupmPfOPmlVbw
> think this is insufficient information.
>
>It should be more clearly highlighted that the NYTAC is proprietary data and it may require a fee of $150-300 to be paid to access, if a non-member of the Linguistic Data Consortium. To say merely “is available upon request” and nothing else is not quite true to my eyes - please warn that it may require payment to access, depending on one's institutional affiliation (or lack thereof). 

**We have updated text to make the fees accessing NYTAC more apparent.**

```diff
- Access to the New York Times Annotated Corpus (NYTAC) is available upon request with the Linguistic Data Consortium at [https://catalog.ldc.upenn.edu/LDC2008T19](https://catalog.ldc.upenn.edu/LDC2008T19).

+ New York Times Annotated Corpus (NYTAC) can be accessed from the Linguistic Data Consortium at [https://catalog.ldc.upenn.edu/LDC2008T19](https://catalog.ldc.upenn.edu/LDC2008T19) where there may be a \$150 to \$300 fee depending on membership status.
```

> is using a proprietary data set that charges for access congruent with the PLOS data availability policy?
>  
> See: "Please note, if data have been obtained from a third-party source, we require that other researchers would be able to access the data set in the same manner as the authors" https://journals.plos.org/plosone/s/data-availability despite that URL indicating just PLOS ONE, the policy applies to all PLOS journals, unless otherwise noted.

**We believe that using the NYTAC dataset does not violate PLOS's data availability policy.**


# Reviewer #2

> Overall, I enjoyed this manuscript for offering a way to quantify the transition of preprints to manuscripts within the biological sciences. Further, the authors develop an approach that could also more generally be useful for classifying biomedical literature, and they even provide as an example a web-based program to find potential publication avenues.

**We are glad you enjoyed reading our manuscript.**

> The methodological approach of the authors is quite unexpected. While I do not see a fundamental flaw in their approach, I would anticipate it to be biased toward the most frequent phrases. When performing computational research there is a risk to pursue analyses through well-intended "improvements" or "customizations" whenever the approach does not seem to yield the expected outcome. As some people could be tempted to interpret parts of the analysis of the authors as warning flags for above having happened, I would recommend adding some additional control analyses and explicit statements about their chosen rationales.
> 
> Particularly, I would be very curious about the discussion, or main text commenting on why the authors created a custom scheme of classifying documents and their similarity based on vectors of words instead of using existing approaches that provide vectors of documents - including doc2vec that is included in the software package that the authors used for word2vec. Do the results change according to the approach?

**Our 'Document embeddings derived from bioRxiv reveal fields and subfields' section was part our motivation for using a linear approach to generate document embeddings.
Our goal was to maximize interpretability of the document embedding space when characterizing preprints within bioRxiv.
We provided word clouds generated from the first prinicpal component to visually see the differences between our linear approach and doc2vec.
Following this analysis we sought to measure the practicality of this embedding space by extending to other applications such as preprint published matching and journal recommendations.
Conversely, we noticed that Doc2Vec had a positive performance outcome for our journal recommendation approach.
We first evaluated these two models using our training dataset, which consisted of randomly holding out published articles and then trying to predict the held out set.
Our next evluation was comparing these two models for our test set, which consisted of using bioRxiv preprints to predict the journal that published their corresponding published counterparts.
We provided the barchart visualization below.
In regards to our test set Doc2vec outperforms our approach for the centroid model but performs evenly for our paper-paper model.
**

**Word2Vec 1st Prinicpal Component WordCloud**
![Word2vec](https://raw.githubusercontent.com/danich1/annorxiver/3bcac4ca2e9249359361525a7e5f3ae36c71d4a5/biorxiv/pca_association_experiment/output/word_pca_similarity/figure_pieces/pca_01_cossim_word_cloud.png)

**Doc2Vec 1st Prinicpal Component WordCloud**
![Doc2vec](https://raw.githubusercontent.com/danich1/annorxiver/3bcac4ca2e9249359361525a7e5f3ae36c71d4a5/biorxiv/pca_association_experiment/output/word_pca_similarity/figure_pieces/pca_01_cossim_word_cloud_doc2vec.png)

**Doc2vec vs Word2vec in Journal Recommendations**
![Doc2vec vs Word2vec Journal Recommendation](https://raw.githubusercontent.com/danich1/annorxiver/13d9789370900a1d04fb296457fd1faf2d76818a/pmc/journal_recommendation/output/figures/doc2vec_word2vec_comparison.png)


> Further, word2vec often seems to work even better when first trained on a larger corpus before then being applied or transferred to more specialized corpora. Personally, I also made this experience when following an example tutorial provided by the creators of the package that the authors used - which too suggests starting with existing pre-trained models. While the more restricted training done by the authors might have reduced the sensitivity of their approach (… which would likely only strengthen their claims), I would be curious whether there was an additional rationale for avoiding the former strategy that might be missed by readers (e.g.: different meanings such as "abstract" that has different meanings for scientists and non-scientists?). 
 
**We chose to use a randomly initialized model as we wanted to take an unbiased approach for generating our document embedding space.
Through this approach, preprints are considered the main factor when analyzing the lingusitic variation contained within each preprint embedding.**

> Likewise, I'm wondering why the authors used a Euclidean distance for word embeddings instead of a Cosine similarity (which if I recall correctly would also be default in the similarity module of the package which the authors used). Cosine similarity should also allow the authors to make statements about the similarity of words without imposing assumptions on similar text lengths or usage frequencies.

**We want to confirm that we have used cosine similarity within our principal component analysis (Figure 2).
We used euclidean distance for our missing link analysis (Figure 3) to highlight that the differece between preprints-published pairs and preprints with a random pair remains regardless of a weaker appraoch.
Regarding our website, we found that using an euclidean distance version of cosine similarity improved our results.
We are updating our resource to reflect these new changes.
**

> Similarly, I was wondering how the "journal-based" approach, which the authors mention briefly against the influence of high publication frequency journals, was implemented. Further, if it could have been avoided by avoiding the Euclidean space.

**Our journal based approach is still required as cosine/euclidean distance only improves jounral matching, whereas the problem of journal overrepresentation will not be resolved by the change.
We handle the issue by calculating a centroid for each journal.
This centroid is calculated via taking the average of every published document present within each journal.
This way every journal has an equal representation for our classifier.**

> The mapping of similarity seems to be based on individual pairs of text and as such it would seem vulnerable of shifting distributions (e.g.: if published articles were somewhat different from preprints, as implied in Figure 1A). I would suspect that the authors would be able to improve their performance even further by doing global matching between many pairs (… again see their adherence to a weaker approach as something that ultimately strengthens their findings). Again, a comment on the rationale of their chosen approach could convey additional non-evident considerations.

**We would like to confirm that we performed a global matching approach when finding missing preprint-publsihed pairs within our missing link analysis (Figure 3).
In regards to our website our classifer compares a query document with all other documents within PMCOA.
This could be considered a global matching approach.**

> I love the web application!

**We are happy you like the application.**

> No statistics are given for the enrichments in Figure 1B-E.

**We report each token with a 95% confidence interval (CI). 
Our frequency counts are sufficiently large that all calculated p-values is approximately or exactly zero.**

> I would welcome a supplemental analysis, that removes single letters and special characters from the analysis of Figure 1B-E as they might change the baseline.

**We have added the results of this request to the supplement.**

> The word cloud of Figure 2B, C is somewhat nice as it shows the main words. However, this information could also be conveyed in the text. Would personally favor to quantitatively see loadings of first few principal components for different terms.

**We have provided a table for the following request in our supplemental section.**

> The definition of "True matches" could be more explicit in within the main text as the preceding figure 3A could for some people set up a different anticipation.

**We agree this term is too vague and we have updated text to be  more explicit.**

```diff
-Approximately 98% of our 200 pairs with an embedding distance in the 0-25th and 25th-50th percentile bins were scored as true matches (Figure 3B).

+Approximately 98% of our 200 pairs with an embedding distance in the 0-25th and 25th-50th percentile bins were successfully matched with their published counterpart (Figure 2B).
```

> The association given in Figure 4A seems to mainly stem from a few papers with large distances. Would an association be present when using the rank-based Spearman correlation instead of a linear regression? Would, for visualization, a logarithmic relationship describe the data better than a linear one?

**We believe there is a misconception for our figure. 
This figure depicts the median halflife publication time for each preprint category within bioRxiv.
**

> I believe that the analysis of Figure 4 B is quite clever as it would seem to address the thinkable concern of preprints with no delay and changes mainly stemming from those manuscripts that were already essentially accepted by manuscripts at the time of posting.

**We are glad you found our analysis insightful.**

> The analysis remarks that for the "Preprints in Motion Collection" the relationship between textual distance and time to publication disappears, and supports this through Figure 6E. However, the background trend in figure 6E includes publications that have been published at a time that exceeds a year. Hence a more faithful comparison would be to censor the background data by a distribution of durations that would correspond to the distribution of durations that would be possible for the "Preprint in Motions Collection" (taking distribution corresponding to interval between their dates on bioRxiv and the time at which authors assessed whether manuscripts were published).

**We have provided a supplemental analysis within our manuscript that shows results after filtering the background distribution based on publication time.**

> Other:
> 
> Labels within figures could often be increased in size to improve readability.

**We have updated the size of our labels for this manuscript.**
 
> The methods section briefly comments on some ambiguous cases for the matching. Would these cases be the result of modifications that defy a 1:1 mapping, e.g.: multiple stories getting fused, or one story getting split?

**Some of these ambigious cases involve abstract or main text changes.
Other cases result in drastically different papers that share similar research content, but are completely different overall.
We provide a table of the ambigious cases we encountered below.**

| biorxiv_doi_url                           | pmcid_url                                   | 
|-------------------------------------------|---------------------------------------------| 
| https://doi.org/10.1101/413450            | https://www.ncbi.nlm.nih.gov/pmc/PMC2967545 | 
| https://doi.org/10.1101/776930            | https://www.ncbi.nlm.nih.gov/pmc/PMC6210049 | 
| https://doi.org/10.1101/2020.01.13.905521 | https://www.ncbi.nlm.nih.gov/pmc/PMC4171638 | 
| https://doi.org/10.1101/352963            | https://www.ncbi.nlm.nih.gov/pmc/PMC6116183 | 
| https://doi.org/10.1101/513002            | https://www.ncbi.nlm.nih.gov/pmc/PMC3545240 | 
| https://doi.org/10.1101/680843            | https://www.ncbi.nlm.nih.gov/pmc/PMC6379322 | 
| https://doi.org/10.1101/074450            | https://www.ncbi.nlm.nih.gov/pmc/PMC5776756 | 
| https://doi.org/10.1101/530758            | https://www.ncbi.nlm.nih.gov/pmc/PMC6663035 | 


> The results of Figure 2A could possibly be strengthened by avoiding Principal Components and replacing them by UMAP projects to account for non-linearity.

**We chose to use PCA for figure 2A as our goal was to visually highlight the concepts captured by our generated prinicpal components.
You can find a umap version of bioRxiv in [this notebook](https://github.com/greenelab/annorxiver/blob/b120488de2c197d93072678f80fce68d11d9e08d/biorxiv/word_vector_experiment/02_biorxiv_visualize_embeddings.ipynb).**

> Although peripheral to the current manuscript, their approach and data would also seem capable to providing an update-able map of the biomedical sciences, by applying their approach of Figure 2 to the PMC corpus data which the authors access too. Such a map could be interesting for those trying to obtain an overview about biology. In case that the authors do not hold plans to publish this elsewhere, and in case that it would be less than a day of work, I would recommend adding such a map to the supplement or as a web service.

**We accomplish this idea with our web application as we provided a 2D visualization of PMC's open access corpus.
This visualziation uses SAUCIE, a autoencoder designed for RNA-seq, instead of UMAP or PCA to generate the landscape.
We also constructed an auto-updater pipeline for this tool so every month new papers are incorporated into our website and our visualization updates accordingly.**

> Are the few publications in Figure 2A, which lie outside of the space that is generally occupied by their respective article categories, somewhat different when doing a superficial manual inspection (e.g.: misclassified by authors, or interdisciplinary research)

**We sampled a select number of neuroscience and bioinformatic articles that were closer to the left side of the figure (PC1 <= -2.5 and -2<PC2<2).
We found that these outliers mainly consisted of interdisciplinary research (e.g. a bioinformatic paper on analyzing flourescence micrographs or a cell biology approach used to analyzer a neuroscience concept).
We provide a table below of preprint dois that fall into this situation.
**

![PCA plot](https://raw.githubusercontent.com/greenelab/annorxiver/51e602d9c4863e1314ed5f01bc483901894ed705/biorxiv/pca_association_experiment/output/pca_plots/svg_files/scatterplot_files/pca01_v_pca02_reversed.svg)

| doi | document category |
| --- | --- |
| 10.1101/075440 | bioinformatics | 
| 10.1101/806216 | bioinformatics |
| 10.1101/696625 | bioinformatics | 
| 10.1101/835181 | bioinformatics | 
| 10.1101/583187 | bioinformatics |
| 10.1101/610196 | neuroscience   |
| 10.1101/2020.01.08.898080 | neuroscience |
| 10.1101/664557 | neuroscience |
| 10.1101/655498 | neuroscience | 
| 10.1101/244111 | neuroscience |

> Adding a few words to "examining the top five and bottom five preprints" could avoid misunderstanding (e.g.: while I suspect that it is the position in Figure 2A, I was first thinking about the most/least successful/downloaded…)

**We have updated the text to be more explicit.**

```diff
- Examining the top five and bottom five preprints within the systems biology field reinforces PC1's dichotomous theme (Table {@tbl:five_pc1_table}).

+ Examining the top five highest-scoring and bottom five lowest-scoring systems biology preprints along PC1 reinforces its dichotomous theme (Supplementary Table {@tbl:five_pc1_table}).
```

> The vector representation of words and documents should allow the authors to quantify shifts that appear between preprints and published manuscripts. Though not necessary from my perspective, many interesting analyses could be done in vector space (e.g.: does language get more positive, or start to refer to more established concepts…?). Maybe there is something small that could be done. Alternatively, the discussion could possibly be extended to demonstrate the implications of vector space, and thus their own work, for future research into preprints and peer review.

**Thank you for pointing out potential extensions to our vector space.
We incorporated these suggestions into our discussion as potential avenues of future work.**

```diff
+ Along with anaylyzing lingusitic variation, future work could utilize this embedding space to quantify sentiment trends such as authors writing preprints with a more positive language over time.
```

> Along above, the discussion could be extended toward prior uses of Word2vec in the studies of science, such as Tshitoyan et al. Nature 2019.

**We have added this citation into our dicussion.**

```diff
+ Furthermore, future applications similar to [@doi:10.1038/s41586-019-1335-8] could be applied to this embedding space.
```

> Repeating the link to the web app in the main text would be convenient.

**We have updated the text to include the web app link throughout our website section.**

> Seeing Figure 6D and 6E, I would enjoy the authors showing or discussing more explicitly, whether textual differences increase with the number of revisions (and/or if there were some more complex changes such as reversions to earlier versions).

**We performed a linear regression analysis to determine how preprint version counts is associated with textual changes changes using all preprint-published pairs within bioRxiv.
We found a positive slope between version count and document distance indicating preprints undergo small textual changes through every new version posted onto bioRxiv.
However, this positive slope is not significant enough to include in our manuscript.
**

![Version Count vs Document distance Linear regression](https://raw.githubusercontent.com/danich1/annorxiver/bc7761c4db132f1287205680a1e2e5f220a85755/biorxiv/publication_delay_experiment/output/version_count_doc_distances.png)

# Reviewer #3
 
> This study asks an important question: (how) do preprints change between their initial release on a preprint server and their eventual publication in a peer-reviewed journal? While the analysis of the linguistic changes doesn't reveal anything particularly exciting (mostly typesetting and references to supplementary information included in response to reviewer requests), this is an incredibly useful result in demonstrating that preprints are typically of high quality, which has broad implications for how researchers and their work are assessed in career, funding, and publishing decisions. The authors have developed some very promising deliverables based on document embeddings that should be broadly applicable to readers, authors, journal editors, and other stakeholders navigating the complex landscape of preprinted and published literature.
>
> Major Comments:
> 
> The method for discovering unannotated preprint-publication relationships is very neat, but I imagine it's rather unwieldy to match a novel publication against the full-text bioRxiv corpus in downstream applications (e.g., bioRxiv's automation)--could this be optimized by reducing the search space to preprints that share some or all of the same authors, within a reasonable date range, and/or only considering paper/preprint metadata (e.g., abstract, title, references)? Such an approach might also enable annotation of preprints that are eventually published as non-OA peer reviewed articles for which such metadata are available.

UPDATE
**We have checked to see if abstracts are possible to use for document matching.
We found..**

 
> Section "Building Classifiers to Detect Linguistically Similar Journal Venues and Published Articles":
> 
> "Specific journals publish articles in a focused topic area, while others publish articles that cover many topics. Likewise, some journals have a publication rate of at most hundreds of papers per year, while others publish at a rate of at least ten thousand papers per year. Accounting for these characteristics, we designed two approaches - one centered on manuscripts and another centered on journals."  << this could use some unpacking and/or reorganizing of details found later in this section--as I understand it, the variation in journals' topical breadth motivates the development of a manuscript-focused classifier (so that topically similar papers appearing in generalist journals do not get obscured) and the variation in journals' publication rates motivates a journal-focused classifier (so that high-output journals do not overwhelm more selective or less popular journals).

**We recognize that this section is a bit dense.
We have have updated our manuscript to unpack this explanation so the rationale for our models is a bit more lucid.**

```diff
+ Training models to identify which journal publishes similar articles is challenging as not all journals are the same. 
+ Some journals have a publication rate of at most hundreds of papers per year, while others publish at a rate of at least ten thousand papers per year.
+ Furthermore, some journals focus on publishing articles within a concentrated topic area, while others cover many dispersive topics.
+ Therefore, we designed two approaches to account for these characteristics.
+ Our first approach focuses on articles that account for a journal's variation of publication topics.
+ This approach allows for topically similar papers to be retrieved independently of their respective journal.
+ Our second approach is centered on journals to account for varying publication rates.
+ This approach allows more selective or less popular journals to have equal representation to their high publishing counterparts.
```

> I'm also curious how often these two classifiers agree--are the top matching papers typically found in the top matching journals? In cases where the two classifiers tend to disagree, are there any common characteristics of the preprints the application is trying to classify?

**We evaluated our classifier agreement by calculating the overlap coefficient between the ten journal recommendations from our centroid based classifer and ten unique journal recommendations from our paper-paper classifier.
We randomly sampled 1700 preprint-published pairs from our test set and calculated coefficient for each pair.
We found that the average coefficient was 0.21.
We generated a random baseline for both of our models to determine how 0.21 compared.
Our random baseline for the centroid classifier consisted of randomly sampling without replacement 10 journals from our sampled datasets.
Using this approach we obtained an overlap coefficient of 0.0184.
Our random baseline for the paper-paper classifier consisted of randomly sampling journals until ten unique journals were obtained.
Using this approach we obtained an overlap coefficient of 0.009.
Overall we can state that our approach agrees better than randomly sampled pairs.
**

> Minor Comments (by section):
> 
> Introduction:
> 
> The references of text mining on biomedical corpora should include Desai et al (2018) [https://www.biorxiv.org/content/10.1101/333922v1.abstract], which describes a similar recommendation engine.

**We have added this reference to our manuscript.**
```diff
- Textual analysis uses linguistic, statistical, and machine learning techniques to analyze and extract information from text [@doi:10.1111/1475-679X.12123].

+ Textual analysis uses linguistic, statistical, and machine learning techniques to analyze and extract information from text [@doi:10.1111/1475-679X.12123; @doi:10.1101/333922].
```

> Section "Comparing Corpora":
> 
> Inconsistent formatting of "spaCy"

**We updated our manuscript to make sure spaCy is properly formatted.**

```diff
- Spacy is a lightweight and easy-to-use python package designed to preprocess and filter text [@spacy2].

+ SpaCy is a lightweight and easy-to-use python package designed to preprocess and filter text [@spacy2].
```

> Define "stopwords," since many readers may be unfamiliar with this term

**We updated our manuscript to have an explanation of "stopwords".**

```diff
+ All corpora contain multiple words that do not have any meaning (e.g. conjunctions, prepositions, etc.) or occur with a high frequency.
+ These words are termed stopwords and are often removed to improve text processing pipelines.
```

> Section "Constructing a Document Representation for Life Sciences Text":
> 
> This switches back to using "words" instead of "tokens" as in the previous section

**Thank you for pointing this out.
We have carefully edited our manuscript to make sure "tokens" was consistently used instead of "words".**
 
> Section "Measuring Time Duration for Preprint Publication Process":
> 
> Does this include the new preprint-publication pairs discovered in the previous section, or only those annotated in the data provided by the bioRxiv API?

**This section only contains preprints pairs that have been established prior to our document matching approach.**

> Section "Preprints with more versions or more text changes took longer to publish":
> 
> Fig. 4: can the longer publication times for scicomm/education papers (Fig 4a) be explained by a tendency to go through more versions (Fig 4b)?

**We cannot accurately answer this question as majority of the published articles in our snapshot aren't contained in Pubmed Central's Open Access Corpus (PMCOA).
However, the preprints that do have a matching counterpart in PMCOA are provided within our supplemental file.
**

> It might be worthwhile to explore what happens post-publication to papers that go through more preprint revisions and take longer to publish, as this could have practical implications for authors as they decide when/if to submit/revise their preprints. Do these papers ultimately receive more citations, end up in journals with higher impact factors, or receive more attention on social media?

**We have provided a supplemental file that contains preprints and their corresponding published information for anyone to easily inspect these changes themselves.**

> Section "Preprints with similar document embeddings share publication venues":
> 
> From personal experience, converting bioRxiv PDFs to text sometimes introduces weird noise and artifacts. Since bioRxiv and medRxiv both offer full-text HTML for many (if not all?) articles, is it possible to modify the application to use this cleaner data source?

**At the time of submission we recognize that using xml is better than solely relying on the pdf parser.
We updated our website to attempt to retrieve the xml version first, then resort to the pdf parser if the xml version is not available.**

> Section "Contextualizing the Preprints in Motion Collection":
> 
> Figure description for Fig 6E is mislabeled as D

**We updated our text to fix this label mismatch.**

> There are several casually/awkwardly-worded or grammatically incorrect sentences throughout that could use some finesse:
> 
> Introduction:
> 
> "We hypothesize that preprints and biomedical text are pretty similar…"
> 
> Measuring Time Duration for Preprint Publication Process:
> 
> "Preprints that are published can take varying amounts of time to be published."
> 
> "We accomplish this by first randomly sampled with replacement a pair of preprints…"
> 
> Building Classifiers to Detect Linguistically Similar Journal Venues and Published Articles:
> 
> "Preprints are more likely to be published in journals that contained similar content to work in question."
> 
> Web Application for Discovering Similar Preprints and Journals:
> 
> "The application downloads a pdf version of any preprint hosted on the bioRxiv or medRxiv server uses PyMuPDF to extract text from the downloaded pdf and feeds the extracted text into our CBOW model to construct a document embedding representation."
> 
> Preprints with more versions or more text changes took longer to publish:
> 
> "Each new version adds additional 51 days before a preprint is published."

**We have updated these sentences to be more clear within our manuscript.**

```diff
- We hypothesize that preprints and biomedical text are pretty similar, especially when controlling for the differential uptake of preprints across fields.

+ We hypothesize that preprints and biomedical text will appear to have similar characteristics, especially when controlling for the differential uptake of preprints across fields.
```

```diff
- Preprints that are published can take varying amounts of time to be published.

+ Preprints can take varying amounts of time to be published.
```

```diff
- We accomplish this by first randomly sampled with replacement a pair of preprints from the Bioinformatics topic area as this was well represented within bioRxiv and contains a diverse set of research articles.

+ We first randomly sampled with replacement a pair of preprints from the Bioinformatics topic area as this was well represented within bioRxiv and contains a diverse set of research articles.
```

```diff
- Preprints are more likely to be published in journals that contained similar content to work in question.

+ Preprints are more likely to be published in journals that publish articles with similar content.
```

```diff
- The application downloads a pdf version of any preprint hosted on the bioRxiv or medRxiv server uses PyMuPDF [@url:https://pymupdf.readthedocs.io/en/latest/intro.html] to extract text from the downloaded pdf and feeds the extracted text into our CBOW model to construct a document embedding representation.

+ Our application attempts to download the full text xml version of any preprint hosted on the bioRxiv or medRxiv server and uses the lxml package (version num) to extract text.
+ If the xml version isn't available our application defaults to downloading the pdf version and uses PyMuPDF [@url:https://pymupdf.readthedocs.io/en/latest/intro.html] to extract text from the pdf. 
+ The extracted text is fed into our CBOW model to construct a document embedding representation.
```

```diff
- Each new version adds additional 51 days before a preprint is published.

+ Every additional preprint version was associated with an increase of 51 days before a preprint was published.
```