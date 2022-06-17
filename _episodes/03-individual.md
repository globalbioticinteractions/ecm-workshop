---
title: "Individual Data Transcriptions Worksheet activity"
teaching: 
exercises: 10
questions:
- "How do I transcribe this?"
- "How do I intrepret the verbatim data?"
objectives:
- "Transcribe the label data"
- "Think about what common association term you would use"
- "Think about how the interaction could be interpreted differently and if there may be a better term"
keypoints:
- "Association data on specimen labels can be highly variable"
- "Matching data to availble terms can be confusing or interpreted differently"

---

### Objectives
-----
> The goal of this exersise is to transcribe the association data from the label images provided and consider not just how you would interpret and classify an interaction, but how someone else may interpret the interaction.


### Getting started
---------------------------------
> Download a copy of the activity spreadsheet to fill in, or open and make a copy you can edit in Google Drive or Google Sheets. 
> * [Excel sheet (.xlsx)](https://github.com/globalbioticinteractions/ecm-workshop/blob/gh-pages/files/1-%20Individual%20Transcription%20Interactions%20Worksheet.xlsx?raw=true)
>  * [Comma delimited (.csv)](https://github.com/globalbioticinteractions/ecm-workshop/blob/gh-pages/files/1-%20Individual%20Transcription%20Interactions%20Worksheet%20-%20Sheet1.csv)
>  * [Google Spreadsheet (make copy or download)](https://docs.google.com/spreadsheets/d/1Avs_gVdz7Dg8KK4AsUzLTed9Lx3bz8grdxfq6ocqJlI/edit?usp=sharing)

> Transcribe the association data from each of the 7 specimen labels provided below into your spreadsheet. You can also open the images up in separate windows or tabs if you prefer with these links:
> * [Specimen 1](https://i.imgur.com/cAT7uPr.jpg) 
> * [Specimen 2](https://github.com/globalbioticinteractions/ecm-workshop/blob/gh-pages/fig/Specimen%20transcription%20%2302.pdf)
> * [Specimen 3](https://github.com/globalbioticinteractions/ecm-workshop/blob/gh-pages/fig/Specimen%20transcription%20%2303.pdf) 
> * [Specimen 4](https://github.com/globalbioticinteractions/ecm-workshop/blob/gh-pages/fig/Specimen%20transcription%20%2304.pdf) 
> * [Specimen 5](https://github.com/globalbioticinteractions/ecm-workshop/blob/gh-pages/fig/Specimen%20transcription%20%2305.pdf) 
> * [Specimen 6](https://github.com/globalbioticinteractions/ecm-workshop/blob/gh-pages/fig/Specimen%20transcription%20%2306.pdf) 
> * [Specimen 7](https://raw.githubusercontent.com/globalbioticinteractions/ecm-workshop/gh-pages/fig/Specimen%20transcription%20%2307.jpg)


### Specimen Images
---------------------------------
> There are 7 different specimen label images with association data to transcribe. 
> Pick the worksheet format above best for you and transcribe the association data into the worksheet. 


> ## `Specimen 1: Transcribe assocation data from label image`
>
> Fill in all columns of the worksheet as appropriate. 
> 
> <img src="https://i.imgur.com/cAT7uPr.jpg" width="800" align="middle"  />
>
{: .challenge}

> ## `Specimen 2: Transcribe assocation data from label image`
>
> Fill in all columns of the worksheet as appropriate. 
> 
> <img src="https://i.imgur.com/u3RbMP6.jpg" width="800" align="middle"  />
>
{: .challenge}

> ## `Specimen 3: Transcribe assocation data from label image`
>
> Fill in all columns of the worksheet as appropriate. 
> 
> <img src="https://i.imgur.com/aPST1Sj.jpg" height="600" align="middle"  />
>
{: .challenge}

> ## `Specimen 4: Transcribe assocation data from label image`
>
> Fill in all columns of the worksheet as appropriate. 
> 
> <img src="https://i.imgur.com/H7DkDqY.jpg" width="800" align="middle"  />
>
{: .challenge}

> ## `Specimen 5: Transcribe assocation data from label image`
>
> Fill in all columns of the worksheet as appropriate. 
> 
> <img src="https://i.imgur.com/iWKnAX1.jpg" width="800" align="middle"  />
>
{: .challenge}

> ## `Specimen 6: Transcribe assocation data from label image`
>
> Fill in all columns of the worksheet as appropriate. 
> 
> <img src="https://i.imgur.com/TVnNaWJ.jpg" width="800" align="middle"  />
>
{: .challenge}

> ## `Specimen 7: Transcribe assocation data from label image`
>
> Fill in all columns of the worksheet as appropriate. 
> 
> <img src="https://i.imgur.com/aKCknj8.jpg" width="800" align="middle"  />
>
{: .challenge}



{% comment %}
> ## `Import into a sqlite database`
---------------------------------
>Databases are a great way to manage large datasets and handle data filtering, sorting and grouping. Sqlite is commonly used with R as it is easily transferable with the R code. We are not going to learn sqlite today, but there are some great Carpentries tutorials to get you started, including the [Introduction to sqlite](https://swcarpentry.github.io/sql-novice-survey/). Let's step through a few commands to see how easy it is to take a CSV file and create a sqlite database.
{: .callout}

~~~
sqlite3 globi.db

.mode csv

.import Ixodes_data_unique.csv interactions

PRAGMA table_info(interactions);

SELECT sourceTaxonGenusName, count(sourceTaxonGenusName) FROM interactions group by sourceTaxonGenusName;

SELECT interactionTypeName, count(interactionTypeName) FROM interactions group by interactionTypeName;

.exit
~~~
{% endcomment %}

## Next Up: Small Group Data Transcriptions

<p class="text-center">
  <a href="https://www.globalbioticinteractions.org/ecm-workshop/04-small-group/index.html">
    <button type="button" class="btn btn-info"> Small Group Data Transcriptions (Worksheet Activity) </button>
  </a>
</p>
<hr/>


<a href="https://parasitetracker.org"><img src="https://i.imgur.com/i7TNiA5.png" class="inline-image" style="height: 5em;"></a> <a href="https://nsf.gov"><img src="https://i.imgur.com/BdaQNEJ.png" class="inline-image" style="height: 6em;"></a> <a href="https://globalbioticinteractions.org"><img src="https://i.imgur.com/6LYylbe.png" class="inline-image" style="height: 5em;"></a>


