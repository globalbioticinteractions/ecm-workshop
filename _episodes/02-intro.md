---
title: "Introduction & Examples"
teaching: 5 minutes
exercises: 0
questions:
- "What will we be doing?"
- "What is the purpose of this exercise?"
objectives:
- "Understand the available ways to get interaction data"
- "Understand the columns of the downloaded data"
keypoints:
- "Association data is not always straight forward"
- "There may be different interpretations of data depending on the provider or user"
---


### Description
-----
> This hands-on exercise was developed to help data providers transcribe specimen-level data that contains information about associated taxa/specimens. This activity will be focused on parasite-host records, and how to consistently capture interaction data from specimen labels. We will examine specimens that vary in quality of available interaction information on the label and practice data transcription and interaction interpretation for downstream integration with GloBI.

{% comment %}
> Some of the different sources of data include natural history collection records, observations extracted from the literature, interaction and network datasets, observations from community science programs and other, larger aggregated datasets.

<img src="https://github.com/globalbioticinteractions/interaction-data-workshop/blob/gh-pages/fig/data-sources.png?raw=true" height="300" align="middle" />
{% endcomment %}


### Objectives
-----
> Navigate to the [GloBI Data Products](https://www.globalbioticinteractions.org/data) page and explore the [Original Data Sources](https://globalbioticinteractions.org/sources).


### Where to find materials for this activity
-----

<img src="https://github.com/globalbioticinteractions/interaction-data-workshop/raw/gh-pages/fig/interaction-data.png" height="800" align="middle"  />

**stable** versions of the data are versioned in the [doi:10.5281/zenodo.3950589](https://zenodo.org/record/3950590) GloBI data publication. A new version is done about every six months.

**snapshot** are the most recent, live data. Thus, this could change daily! Great for exploration and preliminary analysis.

###  How many records are in the GloBI dataset. It is a lot!
-----

~~~
wc -l interactions.csv
~~~

### Data publication
----
> For research or other data intensive project, it is suggested to use GloBI’s stable versioned integrated data published via [doi:10.5281/zenodo.3950589](https://zenodo.org/record/3950590) or create a new data publication that contains the data you are using.


### Other ways of accessing GloBI data
-----
> Exploratory, interactive queries can be executed through SPARQL and Cypher endpoints, GloBI Search/Browse pages, or by using the REST-y GloBI Web API. For those that use R, rglobi is available to explore interaction data. rglobi can also be used to execute Cypher queries. However, it is best to consider these as methods for exploring data rather than data access points. **If you are doing research, download the full dataset and create a version of it**.

> ## `Discussion: Why is it important to version the GloBI data in research?`
> Take a moment to discuss as a group why it is important to version, publish, or archive a copy of the GloBI dataset you use for research. What are some ways to archive datasets?
{: .discussion}

## Next Up: Reviewing the Reviews

If you'd like to follow along while working with the entire dataset, please jump to [Working with the Whole Dataset](../03-ixodes-whole-dataset). 

If you would like to explore GloBI data through the GloBI webpage, please visit lesson episode [Point and Click](../04-ixodes-point-and-click).



