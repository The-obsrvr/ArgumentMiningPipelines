# Designing and Analysing Argument Mining Pipelines: Towards a Comprehensive Assessment

This repository contains the list of AM literature identified and analyzed through the triple-perspective framework.

## Criteria of Literature Selection

### Inclusion Criteria 

- The literature should contain discussion on implementation of two main argument tasks, namely argument identification (or extraction) and relation identification. Emphasis on literature that employ the term AM pipeline in their work.
- Argument Identification includes terms such as argument extraction, argument selection, argument classification.
- Relation identification includes terms such as sentiment identification, stance identification, support / attack identification.

- The literature should contain extraction of argument, or work with data sets developed, from a natural source in a textual format, that is the data has been developed from research work that analyze natural domains such as the scientific domain, the legal domain, the political domain, the social domain, etc. Emphasis is placed on literature that deals with the social and political domain.
Terms included political discourse analysis, social media, speeches, debates, online discussion forums, legal documents, scientific publications, scientific reviews. 


### Exclusion Criteria
- The literature has no clear discussion of the two main argument tasks, in any capacity.
- The work does not source its data from a natural domain.
- The work only discusses the AM pipeline from a conceptual point of view and not from an implementation point of view.


## Obtain Potentially Relevant Literature

### Search Queries

The search query has been drafted keeping three objectives in mind— argument identification task, relation identification task, and the nature of the data (structure or source). Each of these in turn is represented by an individual block or “group” containing the respective key terms that ideally should be used in the document. Primarily two databases, SCOPUS and Web of Science have been used to gather the data. 

The queries were executed on June 15th 2025 and reflect the results from then. 

**Scopus**
```
TITLE-ABS-KEY ( ( "argument mining" OR "argumentation mining" OR "argument unit*" OR "argument identification" OR "argument classification" OR "argument extraction" OR "argument detection" OR "AM pipeline" OR "argument mining pipeline" ) AND ( "data" OR "political" OR "social media" OR "online " OR "debate*" OR "public" OR "discussion*" OR "dialog*" OR "conversation*" ) AND ( "relation*" OR "support*" OR "attack*" OR "stance*" ) ) AND PUBYEAR > 1999 AND ( LIMIT-TO ( DOCTYPE , "ar" ) OR LIMIT-TO ( DOCTYPE , "cp" ) OR LIMIT-TO ( DOCTYPE , "bk" ) OR LIMIT-TO ( DOCTYPE , "ch" ) )
```
- 259 documents retrieved

**Web of Science**
```
TS=( ("argument mining" OR "argumentation mining" OR "argument unit*" OR "argument classification" OR "argument identification" OR "argument extraction" OR "argument detection") AND ("relation*" OR "support*" OR "attack*" OR "stance*") AND ("data" OR "political" OR "social media" OR "public" OR "online" OR "debates" OR "dialog*" OR "discussion*" OR "conversation*") ) AND PY=(2000-2025)
```
- 182 documents retrieved.
  
Further refined on document types “Article” and “Meeting”
Contains “meeting” document type, which means not all documents have been peer reviewed, usually are conference papers which are often shorter than journal articles, limiting the quality and depth of research accessible. But given that argument mining is quite a niche and small community (with majority of the work emerging from workshops and niche conferences) we kept them in the analysis as long as they satisfied our selection criteria.

Other databases under consideration include “Semantic Scholar”, “Google Scholar”, “ACL Anthology” etc. but most of them have been covered by SCOPUS and WoS.

## Selection of Relevant Literature

Merge the different databases

- Assigning unique ID
- Removing duplicates: title or abstract are similar. 

After the merge and duplicate removal, 378 documents were retained.

Next, we filter out entries that do not meet our criteria. We take the help of an LLM and instruct it with the following prompt that contains our selection criteria:

```
```

We then manually inspect the output produced by the LLM for correctness and filter out entries where certain information cannot be immediately perceived from the abstract. In some exceptional cases, we consider reviewing the rest of the paper (if it is open-access) to see if it meets our selection criteria. By the end we are left with around **150** documents for our analysis.


## Triple-perspective Framework

We apply our triple-perspective framework, detailed in the paper, to list how the pipelines model, operationalize, and contextualize argument structures within a domain. 

For this effort, we employ our guiding questions onto the selected relevant literature and note the most representative literature.

### Linguistic Perspective

### Computational Perspective

### Domain Perspective


## To Cite this work

{}











