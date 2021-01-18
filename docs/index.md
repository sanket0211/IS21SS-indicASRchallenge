---
layout: workshop      # DON'T CHANGE THIS.
# More detailed instructions (including how to fill these variables for an
# online workshop) are available at
# https://carpentries.github.io/workshop-template/customization/index.html
venue: "Interspeech 2021 Special Session"        # brief name of the institution that hosts the workshop without address (e.g., "Euphoric State University")
address: ""      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria"), videoconferencing URL, or 'online'
country: "in"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes) for the institution that hosts the workshop
language: "in"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the
latitude: "45"        # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "-1"       # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: ""    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: ""    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate:       # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate:         # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
# instructor:  # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper:      # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
email: ["is21ss.indicasrchallenge@gmail.com"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
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
8< ============= For a workshop delete from here =============
For a workshop please delete the following block until the next dashed-line
{% endcomment %}




{% comment %}
8< ============================= until here ==================
{% endcomment %}


{% comment %}
Check DC curriculum
{% endcomment %}



{% comment %}
Check SWC curriculum
{% endcomment %}

{% if site.carpentry == "swc" %}
{% unless site.curriculum == "swc-inflammation" or site.curriculum == "swc-gapminder" %}

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


<p>
  Recently, there have been increasing interests in multilingual automatic speech recognition (ASR) where a speech recognition system is built to cater to multiple low resource languages by taking advantage of low amount of labeled corpora in multiple languages. On the other hand, with multilingualism becoming common in today’s world, there has been increasing interest in code-switching ASR as well. In code-switching, multiple languages are freely interchanged within a single sentence or between sentences. We would like to propose a special session and challenge in Interspeech 2021 on multilingual and code-switching ASR for low resource Indian languages, which have not been widely explored. The success of low-resource multilingual and code-switching ASR often depends on the variety of languages in terms of their acoustics, linguistic characteristics as well as amount of data available and how these are carefully considered in building the ASR system. In this challenge, we would like to focus on building multilingual and code-switching ASR systems through two different sub-tasks related to a total of seven Indian languages with constraints on the data available for acoustic modeling and language modeling.

</p>
<p> </p> 
<p>
  India is a country of language continuum, where every few kilometers the dialect/language changes. Various language families or genealogical types have been reported, in which the vast number of Indian languages can be classified, including Austro-Asiatic, Dravidian, Indo-Aryan, Tibeto-Burman and more recently, Tai-Kadai and Great Andamanese. However, there are no boundaries among these language families, rather languages across different language families share linguistic traits including retroflex sounds, SOV word order, absence of prepositions and many more resulting in acoustic and linguistic richness. According to the 2001 census, 29 Indian languages have more than a million speakers. Among these, 22 languages have been given the status of official languages by the Government of India. Most of these languages are low resource. Many of these languages do not have a written script and hence, speech technology solutions would greatly benefit such communities. Code-switching between an Indian language and (Indian) English has been a normal feature of everyday speech. Understanding code-switching patterns in different languages and developing accurate code-switching ASR remain a challenge due to the lack of large code-switched corpora. Thus, techniques that exploit unique properties and similarities among the Indian languages could be useful for building multilingual and code-switching ASR systems in these resource constrained settings.

</p>
<p> </p> 
<p>
  We will be providing a total of 630 hours of data in six Indian languages, namely, Hindi, Marathi, Odia, Bengali, Telugu, Tamil and Gujarati. This includes code-switched transcribed speech in two code-switched language pairs, Hindi-English and Bengali-English. Domains of the speech recordings vary across different languages.  </p>
  <p> </p> 
  <p>
  For example, the Odia data comes from healthcare, agriculture and financial domains. The Hind-English and Bengali-English data are drawn from a repository of technical lectures on a diverse range of topics in computer science. For more description on this, please refer to the Dataset section <LINK>. The participants in this challenge will be required to use only the released data to build ASR systems in these languages, which will make the task fair for all participants and direct the focus of the work to the low resource setting. However, we will not restrict participants from only working on one of the components of the multilingual and code-switching ASR pipeline – participants will be free to innovate in any aspect of the multilingual and code-switching ASR system as long as they only use the data provided.  We will release a baseline system that participants can compare their systems against and use as a starting point.  During testing, we will release a held-out blind test set that the systems will be evaluated on.
  </p>
  <p> </p> 
  <h3> The challenge comprises two sub-tasks as described below </h3>
  
  <h4> <b> Sub-task1 </b> </h4>
This sub-task involves building a multilingual ASR system in six languages, namely, Hindi, Marathi, Odia, Telugu, Tamil, and Gujarati. The blind test set will comprise recordings from a subset (or all) of these six languages

<h4> <b> Sub-task2 </b> </h4>
This sub-task involves building a code-switching ASR system separately for Hindi-English and Bengali-English code-switched pairs. The blind test set will comprise recordings from these two code-switched language pairs.

<p> Submissions to this special session should show results on one or more of the above mentioned tasks. Submissions on any topic related to building multilingual code-switching ASR are welcome. This includes (but is not limited to):
</p>
<ul>
  <li> Acoustic modeling for multilingual ASR models </li>
  <li> Language modeling for multilingual ASR models </li> 
  <li> Multilingual ASR model for code-switching </li> 
  <li> Language modeling for code-switching </li> 
  <li> Linguistically informed models for code-switching </li> 


  

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
  
</p>
{% elsif online == "true_public" %}
<p id="where">
  
</p>
{% elsif online == "true_private" %}
<p id="where">
 
</p>
{% endif %}

{% comment %}
DATE

This block displays the date and links to Google Calendar.
{% endcomment %}
{% if page.humandate %}
<p id="when">

</p>
{% endif %}

{% comment %}
SPECIAL REQUIREMENTS

Modify the block below if there are any special requirements.
{% endcomment %}



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


{% endcomment %}

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


<h2 id="schedule"> Important Dates </h2>

{% if site.carpentry == "swc" %}
{% include swc/schedule.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/schedule.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/schedule.html %}
{% endif %}

<hr/>

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

