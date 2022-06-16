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

<img src="https://i.imgur.com/o5jFz1Z.jpg" height="800" align="middle"  /> 

												
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTfWe2BGVRMVRm_7jtDY9QbiJWBN1jSGIEsPBJt5aLC5q0IdwcBdcenW7CsEXFq9l-huuB1FyE27NuI/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTfWe2BGVRMVRm_7jtDY9QbiJWBN1jSGIEsPBJt5aLC5q0IdwcBdcenW7CsEXFq9l-huuB1FyE27NuI/pub?gid=0&single=true&output=pdf"></iframe>




| Image number | Verbatim Interaction Text (Interaction as on label without interpretation)| Human derived/ interpreted interaction | Specimen Taxon name |
|--------------|---------------------------------------------------------------------------|----------------------------------------|---------------------|
|example 1|Lone Star Tick pulled from Susan ~6am 6/25/07 probably attached herself 6/24/07|parasite of|Amblyomma americanum|



-----

### Example 2.
-----

<img src="https://i.imgur.com/G2SW2IZ.jpg" height="400" align="middle"  /> 


## Next Up: Individual Specimen Data Transcriptions

➡️ [Individual Data Transcriptions (Worksheet Activity)](../03-individual). 





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


