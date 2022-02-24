---
title: "Who has a voice in the media ? An EPFL project to discover who to be quotes in newspapers "
layout: post
date: 2021-12-20 12:00
tag: DataViz, WebDev, Python, API
image: /assets/images/wordcloud-speakers-blue-hq.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: ""
category: project
author: eliott
externalLink: false
---
This is a project carried out for the [Applied Data Analysis](https://edu.epfl.ch/coursebook/en/applied-data-analysis-CS-401) course at EPFL.  
Made in collaboration with [Thomas Benchetrit](https://www.linkedin.com/in/thomas-benchetrit/), [Matheus Bernat](https://www.linkedin.com/in/matheus-bernat/), and [Benjamin Hansson](https://www.linkedin.com/in/benjamin-hansson-39b391140/).  
See the website: [https://quotebankers.github.io/](https://quotebankers.github.io/)


---

Isn't it a pleasure to be listened to? The ability to make your voice heard is a privilege that few have. Sometimes you can have the feeling that only the loudest are listened to. Using the Quotebank dataset from 2015 to 2020 and information about the speakers exctracted from Wikidata, we were able to dissect : 
- **WHO** you need to be to be quoted (age, gender, occupation)
- **WHAT** you need to say (which subject to talk about)
- **HOW** you need to talk about it (which emotion to use)

Once a primary analysis was done on the speakers on themselves, a **K-means** clustering algorithm was run on the data to cluster the speakers into sub-groups to be further and deeper analyzed. Then, in order to extract the topic and the emotion for each quote, we used a zero-shot classificatino approach based on the **DistilBERT** base model uncased. This model is fine-tuned on Multi-Genre Natural Language Inference (MNLI) dataset for the zero-shot classification task.
In order to present our results, a **[website](https://quotebankers.github.io/)** was developped using Jekyll. All visualisations were done using plotly. To make the content more interactive and more appealing to users, a **[webapp](https://quotebankers.netlify.app/)** was also developped.

Developped using ReactJS and Material-UI, this app asks you who you are, what you want to talk about and with which emotion in order to predict a *quotation score* which is computed using a Deep Learning model made with TensorFlow and trained on the newly-labelled QuoteBank dataset.
An API was developped with the Flask framework in order to host the predictive model and answer the requests made in the webapp.


---

### About this project
* Python, Javascript
* Packages/Librairies: Pandas, skLearn, plotly, TensorFlow, ReactJS, Flask 
* Interactive webapp, identity and topic oriented analysis of the QuoteBank dataset


### Links
* Link to the [website](https://quotebankers.github.io/). 
* Link to the [webapp](https://quotebankers.netlify.app/)
* Link to the [repositories](https://linktr.ee/QuoteBankers)
* You can find the QuoteBank dataset [here](https://dlab.epfl.ch/people/west/pub/Vaucher-Spitz-Catasta-West_WSDM-21.pdf )
