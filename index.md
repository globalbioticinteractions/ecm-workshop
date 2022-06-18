---
layout: workshop      # DON'T CHANGE THIS.
# More detailed instructions (including how to fill these variables for an
# online workshop) are available at
# https://carpentries.github.io/workshop-template/customization/index.html
venue: "Entomology Collections Management Association Data Workshop"        # brief name of the institution that hosts the workshop without address (e.g., "Euphoric State University")
address: "in-person @ ASU | online"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria"), videoconferencing URL, or 'online'
country: "FIXME"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes) for the institution that hosts the workshop
language: "FIXME"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the
latitude: "45"        # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "-1"       # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "22 June 2022"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "2-4p Mountain Standard Time"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2022-06-22      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2022-06-22        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Erika Tucker", "Jorrit Poelen", "Katja Seltmann", "Kathryn Sullivan", "Jennifer Zaspel"] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper: [ "you!" ]

# ["helper one", "helper two"]     # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
email: ["seltmann@ccber.ucsb.edu","jhpoelen@jhpoelen.nl"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
collaborative_notes:  # optional: URL for the workshop collaborative notes, e.g. an Etherpad or Google Docs document (e.g., https://pad.carpentries.org/2015-01-01-euphoria)
eventbrite:           # optional: alphanumeric key for Eventbrite registration, e.g., "1234567890AB" (if Eventbrite is being used)
---

{% comment %} See instructions in the comments below for how to edit specific sections of this workshop template. {% endcomment %}

{% comment %}
HEADER

Edit the values in the block above to be appropriate for your workshop.
If the value is not 'true', 'false', 'null', or a number, please use
double quotation marks around the value, unless specified otherwise.
And run 'make workshop-check' *before* committing to make sure that changes are good.
{% endcomment %}


{% comment %}
{% endcomment %}


{% comment %}
Check DC curriculum


{% if site.carpentry == "dc" %}
{% unless site.curriculum == "dc-ecology" or site.curriculum == "dc-genomics" or site.curriculum == "dc-socsci" or site.curriculum == "dc-geospatial" %}
<div class="alert alert-warning">
It looks like you are setting up a website for a Data Carpentry curriculum but you haven't specified the curriculum type in the <code>_config.yml</code> file (current value in <code>_config.yml</code>: "<strong>{{ site.curriculum }}</strong>", possible values: <code>dc-ecology</code>, <code>dc-genomics</code>, <code>dc-socsci</code>, or <code>dc-geospatial</code>). After editing this file, you need to run <code>make serve</code> again to see the changes reflected.
</div>
{% endunless %}
{% endif %}
{% endcomment %}


{% comment %}
Check SWC curriculum
{% endcomment %}

{% if site.carpentry == "swc" %}
{% unless site.curriculum == "swc-inflammation" or site.curriculum == "swc-gapminder" %}
<div class="alert alert-warning">
It looks like you are setting up a website for a Software Carpentry curriculum but you haven't specified the curriculum type in the <code>_config.yml</code> file (current value in <code>_config.yml</code>: "<strong>{{ site.curriculum }}</strong>", possible values: <code>swc-inflammation</code>, or <code>swc-gapminder</code>). After editing this file, you need to run <code>make serve</code> again to see the changes reflected.
</div>
{% endunless %}
{% endif %}

{% comment %}
EVENTBRITE

This block includes the Eventbrite registration widget if
'eventbrite' has been set in the header.  You can delete it if you
are not using Eventbrite, or leave it in, since it will not be
displayed if the 'eventbrite' field in the header is not set.
{% endcomment %}
{% if page.eventbrite %}
<strong>Some adblockers block the registration window. If you do not see the
  registration box below, please check your adblocker settings.</strong>
<iframe
  src="https://www.eventbrite.com/tickets-external?eid={{page.eventbrite}}&ref=etckt"
  frameborder="0"
  width="100%"
  height="280px"
  scrolling="auto">
</iframe>
{% endif %}


<h2 id="general">General Information</h2>

{% comment %}
INTRODUCTION

Edit the general explanatory paragraph below if you want to change
the pitch.
{% endcomment %}

This Carpentries workshop activity is part of the 4th offering of the Entomological Collections Management (ECM) Workshop. This hybrid model workshop activity will be held both in-person at Arizona State University (ASU) in Tempe, Arizona and virtually on June 22nd. The full ECM Workshop is from June 20-24, 2022 and is also following a hybrid model (on-site events begin the evening of the 19th) (see the [ECM Workshop site](https://ecnweb.net/workshop/)).

❗**Important time zone note**❗ The live work shop session is in Arizona. Most of **Arizona does _not_ follow daylight savings time**, they are on Mountain Standard Time (GMT-7) (not to be confused with Mountain Daylight time or Mountain Time which is the first thing that comes up on Google). This means, during June, participants on EDT (GMT-4) have a 3 hour different (Washington DC), CST (GMT-5) a 2 hour differnce (Chicago), MDT (GMT-6) a 1 hour difference (Denver), and PDT (GMT-7) is currently in the same time zone (Los Angeles). This will change in the fall when daylight saving time ends for most folks. For additional time zones please check out one of these free world time zone converters:
* [Time and Date](https://www.timeanddate.com/worldclock/converter.html?iso=20220617T163000) (can add multiple times and places)
* [24 Times Zones](https://24timezones.com/difference)

Join Erika Tucker and Jorrit Poelen for an examination of specimen association data and terminology followed by discussion on interpretations and downsteam usage. 

During this one-hour long, participatory workshop for collection managers, collection caretakers, and anyone interested in learning about association data, we will examine label data from real specimens in collections that have association data.  We will discuss commonly used terms one may encounter in many databases, potential interpretations, and how best to capture data so that is usable by researchers and data users downstream. 

This workshop is open to anyone interested in biotic or species interaction data even if you are presently not using GloBI. We will highlight data from the Terrestrial Parasite Tracker project, but the methods are available for anyone interested in biotic interactions (see more at https://www.globalbioticinteractions.org/sources).

The proposed outcome of this workshop is to gain a better understanding of biotic association data, how it can be interpreted, and how it may be used in the future. We will work together through a series of exploratory data exercises. No programming experience is required, and you will use your own device to download data and create Google Sheets if you are attending virtually. If you are attending in-person, physical images and worksheets will be handed out. Everyone will contribute during this workshop. 

<hr/>

{% comment %}
SCHEDULE

Show the workshop's schedule.

Small changes to the schedule can be made by modifying the
`schedule.html` found in the `_includes` folder for your
workshop type (`swc`, `lc`, or `dc`). Edit the items and
times in the table to match your plans. You may also want to
change 'Day 1' and 'Day 2' to be actual dates or days of the
week.

For larger changes, a blank template for a 4-day workshop
(useful for online teaching for instance) can be found in
`_includes/custom-schedule.html`. Add the times, and what
you will be teaching to this file. You may also want to add
rows to the table if you wish to break down the schedule
further. To use this custom schedule here, replace the block
of code below the Schedule `<h2>` header below with
`{% include custom-schedule.html %}`.
{% endcomment %}

<h2 id="schedule">Schedule Group 1</h2>

{% include custom-schedule.html %}

<h2 id="schedule">Schedule Group 2</h2>

{% include custom-schedule2.html %}

<hr/>

{% comment %}
SETUP

Delete irrelevant sections from the setup instructions.  Each
section is inside a 'div' without any classes to make the beginning
and end easier to find.

This is the other place where people frequently make mistakes, so
please preview your site before committing, and make sure to run
'tools/check' as well.
{% endcomment %}

<h2 id="setup">Setup</h2>

<p>
  To participate in this
  {% if site.carpentry == "swc" %}
  Software Carpentry
  {% elsif site.carpentry == "dc" %}
  Data Carpentry
  {% elsif site.carpentry == "lc" %}
  Library Carpentry
  {% endif %}
  workshop,
  you will need internet access and the ability to download spreadsheet files (.xlsx or .csv) or to use spreadsheet files in <a href = "https://www.google.com/sheets/about/">Google Doc/Sheets</a>.

  In addition, you will need an up-to-date web browser.
</p>
<p>
  We maintain a list of common issues that occur during installation as a reference for instructors
  that may be useful on the
  <a href = "{{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions">Configuration Problems and Solutions wiki page</a>.
</p>

{% comment %}
For online workshops, the section below provides:
- installation instructions for the Zoom client
- recommendations for setting up Learners' workspace so they can follow along
  the instructions and the videoconferencing

If you do not use Zoom for your online workshop, edit the file
`_includes/install_instructions/videoconferencing.html`
to include the relevant installation instrucctions.
{% endcomment %}
{% if online != "false" %}
{% include install_instructions/videoconferencing.html %}
{% endif %}

{% comment %}
These are the installation instructions for the tools used
during the workshop.
{% endcomment %}

{% if site.carpentry == "swc" %}
{% include swc/setup.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/setup.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/setup.html %}
{% elsif site.carpentry == "pilot" %}
Please check the "Setup" page of
[the lesson site]({{ site.lesson_site }}) for instructions to follow
to obtain the software and data you will need to follow the lesson.
{% endif %}

{% comment %}
LOCATION

This block displays the address and links to maps showing directions
if the latitude and longitude of the workshop have been set.  You
can use https://itouchmap.com/latlong.html to find the lat/long of an
address.
{% endcomment %}
{% assign begin_address = page.address | slice: 0, 4 | downcase  %}
{% if page.address == "online" %}
{% assign online = "true_private" %}
{% elsif begin_address contains "http" %}
{% assign online = "true_public" %}
{% else %}
{% assign online = "false" %}
{% endif %}
{% if page.latitude and page.longitude and online == "false" %}
<p id="where">
  <strong>Where:</strong>
  {{page.address}}.
  Get directions with
  <a href="//www.openstreetmap.org/?mlat={{page.latitude}}&mlon={{page.longitude}}&zoom=16">OpenStreetMap</a>
  or
  <a href="//maps.google.com/maps?q={{page.latitude}},{{page.longitude}}">Google Maps</a>.
</p>
{% elsif online == "true_public" %}
<p id="where">
  <strong>Where:</strong>
  online at <a href="{{page.address}}">{{page.address}}</a>.
  If you need a password or other information to access the training,
  the instructor will pass it on to you before the workshop.
</p>
{% elsif online == "true_private" %}
<p id="where">
  <strong>Where:</strong> This training will take place online.
  The instructors will provide you with the information you will need to connect to this meeting.
</p>
{% endif %}

{% comment %}
DATE

This block displays the date and links to Google Calendar.
{% endcomment %}
{% if page.humandate %}
<p id="when">
  <strong>When:</strong>
  {{page.humandate}}.
  {% include workshop_calendar.html %}
</p>
{% endif %}

{% comment %}
SPECIAL REQUIREMENTS

Modify the block below if there are any special requirements.
{% endcomment %}
<p id="requirements">
  <strong>Requirements:</strong>
  {% if online == "false" %}
    Online participants must bring a laptop with a
    Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.) that they have administrative privileges on.
  {% else %}
    Online participants must have access to a computer with a
    Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.) that they have administrative privileges on for downloading purposes.
  {% endif %}
  Internet access and the ability to download worksheets (or copy the templates into Google Sheets) is required. 
</p>

{% comment %}
ACCESSIBILITY

Modify the block below if there are any barriers to accessibility or
special instructions.
{% endcomment %}

<p id="accessibility">
  <strong>Accessibility:</strong>
{% if online == "false" %}
  We are committed to making this workshop
  accessible to everybody. The workshop organizers have checked that:
</p>
<ul>
  <li>The room is wheelchair / scooter accessible.</li>
  <li>Accessible restrooms are available.</li>
</ul>
<p>
  Digital materials will be provided in advance of the workshop and
  large-print handouts are available for in-person attendies. If additional help is needed, please notify the
  organizers in advance.  If we can do something to help make learning easier for
  you (e.g. sign-language interpreters, lactation facilities) please
  get in touch (using contact details below) and we will
  attempt to provide them.
</p>
{% else %}
  We are dedicated to providing a positive and accessible learning environment for all. Please
  notify the instructors in advance of the workshop if you require any accommodations or if there is
  anything we can do to make this workshop more accessible to you.
</p>
{% endif %}

{% comment %}
CONTACT EMAIL ADDRESS

Display the contact email address set in the configuration file.
{% endcomment %}

<p id="contact">
  <strong>Contact:</strong>
  Please email
  {% if page.email %}
  {% for email in page.email %}
  {% if forloop.last and page.email.size > 1 %}
  or
  {% else %}
  {% unless forloop.first %}
  ,
  {% endunless %}
  {% endif %}
  <a href='mailto:{{email}}'>{{email}}</a>
  {% endfor %}
  {% else %}
  to-be-announced
  {% endif %}
  for more information.
</p>

<p id="roles">
  <strong>Roles:</strong>
  To learn more about the roles at the workshop (who will be doing what),
  refer to <a href="https://carpentries.org/workshop_faq/#what-are-the-roles-of-everyone-participating-in-a-workshop">our Workshop FAQ</a>.
</p>

{% comment %}
WHO CAN ATTEND?

If you would like to specify who can attend the workshop,
you can use the section below.

Move the 'endcomment' tag above the beginning of the following
<p> tag to make this section visible.

Edit the text to match who can attend the workshop. For instance:
- This workshop is open to affiliates to ABC university.
- This workshop is open to the public.
- If you are interested in attending this workshop, contact me@example.com
  for more information

<p id="who-can-attend">
    <strong>Who can attend?:</strong>
    This workshop is open to ....
</p>
{% endcomment %}

<hr/>


<h2 id="Acknowledgements">Acknowledgements</h2>

This workshop is supported through the <img src="fig/nsf_logo.png" class="inline-image"> [National Science Foundation](https://nsf.gov) award "Towards a Sustainable Management of Insect Collections in the U.S. through the Entomological Collections Management Workshop," Award number [DBI:1640919](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1640919) Additional support is provided by the <img src="fig/parasite_tracker_logo.png" class="inline-image"> [Terrestrial Parasite Tracker](https://parasitetracker.org) project through the <img src="fig/nsf_logo.png" class="inline-image"> [National Science Foundation](https://nsf.gov) award "Collaborative Research: Digitization TCN: Digitizing collections to trace parasite-host associations and predict the spread of vector-borne disease," Award numbers [DBI:1901932](https://nsf.gov/awardsearch/showAward?AWD_ID=1901932&HistoricalAwards=false) and [DBI:1901926](https://nsf.gov/awardsearch/showAward?AWD_ID=1901926&HistoricalAwards=false). 

Big thanks to Kat Sullivan (MPM/TPT) for providing excellent workshop/lesson content and templates, and to all the <img src="fig/globi_logo.png" class="inline-image">[GloBI partners](https://globalbioticinteractions.org/about#partners) for their support.

A special thanks to the thousands of (citizen) scientists and their institutions for openly sharing their [datasets](https://globalbioticinteractions.org/sources). Also, thanks to the thousands of software engineers for providing high quality open source software on which GloBI and this Carpentries lessions is built . 

<a href="https://parasitetracker.org"><img src="fig/parasite_tracker_logo.png" class="inline-image" style="height: 5em;"></a> <a href="https://nsf.gov"><img src="fig/nsf_logo.png" class="inline-image" style="height: 6em;"></a> <a href="https://globalbioticinteractions.org"><img src="fig/globi_logo.png" class="inline-image" style="height: 5em;"></a>

{% comment %}
I don't think iDigBio really did anything for the workshop... It can be added back in though. 
<a href="https://www.idigbio.org/"><img src="fig/idigbio_logo.png" class="inline-image" style="height: 4em;"></a> 
{% endcomment %}

<hr/>

{% comment%}
CODE OF CONDUCT
{% endcomment %}

<h2 id="code-of-conduct">Code of Conduct</h2>

<p>
Everyone who participates in Carpentries activities is required to conform to the <a href="https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html">Code of Conduct</a>. This document also outlines how to report an incident if needed.
</p>

<p class="text-center">
  <a href="https://goo.gl/forms/KoUfO53Za3apOuOK2">
    <button type="button" class="btn btn-info">Report a Code of Conduct Incident</button>
  </a>
</p>
<hr/>


{% comment %}
Collaborative Notes

If you want to use an Etherpad, go to

https://pad.carpentries.org/YYYY-MM-DD-site

where 'YYYY-MM-DD-site' is the identifier for your workshop,
e.g., '2015-06-10-esu'.

Note we also have a CodiMD (the open-source version of HackMD)
available at https://codimd.carpentries.org
{% endcomment %}
{% if page.collaborative_notes %}
<h2 id="collaborative_notes">Collaborative Notes</h2>

<p>
We will use this <a href="{{ page.collaborative_notes }}">collaborative document</a> for chatting, taking notes, and sharing URLs and bits of code.
</p>
<hr/>
{% endif %}


## Recording

A recording of this workshop will be added after the event in this location.

{% comment %}
You can find a mp4 recording of the 2021-04-28 event via:

> Seltmann & Poelen. 2021. A Practical Exploration of Biotic Interaction Data Management and Information Retrieval through Terrestrial Parasite Tracker (TPT) and Global Biotic Interactions (GloBI) [Workshop]. Zenodo. [doi:10.5281/zenodo.4759060](https://doi.org/10.5281/zenodo.4759060) 

or streaming online on Vimeo at:

<iframe src="https://player.vimeo.com/video/546669878" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/546669878">A Practical Exploration of Biotic Interaction Data Management and Information Retrieval through TPT and GloBI</a> from <a href="https://vimeo.com/idigbio">iDigBio</a> on <a href="https://vimeo.com">Vimeo</a>.</p>
{% endcomment %}

<hr/>


## Disclaimer

Note that this is not (yet) an official Carpentries workshop, but we are working towards becoming one.

{% comment %}
AUDIENCE

Explain who your audience is.  (In particular, tell readers if the
workshop is only open to people from a particular institution.
{% endcomment %}
{% if site.carpentry == "swc" %}
{% include swc/who.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/who.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/who.html %}
{% endif %}
