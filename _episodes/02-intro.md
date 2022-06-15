---
title: "Introduction & Examples"
teaching: 5 minutes
exercises: 0
questions:
- "What will we be doing?"
- "What is the purpose of this exercise?"
objectives:
- "Explain activity"
- "Go over example specimens"
- "Provide materials for workshop activity"
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
> 1. Gain a better understanding of parasite collections interactions data
> 2. Practice transcribing specimen interactions data using real examples
> 3. Discuss (first in small groups, then as a network) different ways in which species interactions data can be interpreted 
> 4. Compile a list of verbatim terms currently used to describe associations on specimen labels 
> 5. Compile a set of ‘interaction types’ derived from ‘human interpreted interactions’
> 6. Share outcomes (e.g., interactions translation table)


### Where to find materials for this activity
-----

TODO: Add links... Screenshot? 
<img src="https://github.com/globalbioticinteractions/interaction-data-workshop/raw/gh-pages/fig/interaction-data.png" height="800" align="middle"  />


### Example 1.
-----

<img src="https://github.com/globalbioticinteractions/ecm-workshop/blob/gh-pages/_episodes/Example1.JPEG" height="800" align="middle"  /> 

												


### Example 2.
-----

<img src="https://github.com/globalbioticinteractions/ecm-workshop/blob/gh-pages/_episodes/Example2.jpg" height="800" align="middle"  /> 


## Next Up: Individual Specimen Data Transcriptions

[Individual Data Transcriptions (Worksheet Activity)](../03-individual). 





{% comment %}
Material from copied template (just case wat to copy any formatting later..)

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

{% endcomment %}


