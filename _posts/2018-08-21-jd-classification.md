---
title: "How do employers distinguish Data Scientists and Data Analysts?"
date: 2018-08-21
tags: [Classification, Python, Naive Bayes]
excerpt: "A model that predicts the title from just the job description."
mathjax: true
---

## Motivation
Being a data practioner, I often get asked the question *What is the difference between a Data Scientist and a Data Analyst?* Though I usually answer this question empirically, I decided to take a data-driven approach and build a model to more systemtically identify the distinction between these two roles. 

## Overview
What I ended up doing was collecting job descriptions for Data Scientist and Data Analyst roles posted by the big tech companies in Silicon Valley on job boards and training a model on a subset to see if I could accurately predict the remaining titles from just the job descriptions. 

I ended up training a Multinomial Naives Bayes model to predict the job titles. My final model had an **ROC AUC of 88%**, meaning my model did fairly well to account for both the true positive rate (sensitivity) and the false positive rate (100-specificity). Unsurprisingly, the top key words/phrases for Data Scientist were: *machine learning*, *models*, *algorithms* while that for Data Analysts were: *reports*, *dashboards*, and *excel*. 

## Takeaways
**Examining the results that my model classified incorrectly actually gives insight into employers and their expectations.**

There are several reasons why a company might choose to display a title where the description does not match the role. Lyft, for example, on their blog, wrote the following article [What's in a name?](https://eng.lyft.com/whats-in-a-name-ce42f419d16c), where they explained that they strategically chose to change the title of a Data Analyst to a Data Scientist to retain talent (in my model, this role comes up as a false negative). However, instead of encompassing both roles in one title, they updated that of Data Scientist to research scientist. Others have done it to attract talent and get a pool of applicants that are simply drawn to the [Sexiest Job of the 21st Century](https://hbr.org/2012/10/data-scientist-the-sexiest-job-of-the-21st-century), as proclaimed by Harvard Business Review. While others have changed the title to Data Scientist, but kept the Data Analyst description to attract more skilled workers.

I am curious if other companies will follow this example and broaden the definition of a Data Scientist. Will more companies use these two terms interchangeably or create new terminology like research scientist?

**Frequent terms establish the baseline knowledge expected in both roles, while frequent but unique terms per role highlight key differences.**
 
It is no surprise that *SQL* and *analysis* show up frequently in both postings (see chart below). What is interesting, however, is that *statistics* shows up in both. Context is very important; the words that show up surrounding this term provide additional information about the level of expertise required. Upon further inspection, it looks like this term frequently shows up alongside a list of other quantitative degrees, for both roles, so it is less surprising than it was at initial glance. 

Another term that appears frequently for both is *Python*. The frequency of which this word shows up for Data Scientist roles is, however, considerably higher than the times it appears in Data Analyst JDs. Almost 90% of the data science roles contain the key term, while only 60% of the Data Analyst JDs have it, indicating that Python is an expected skill for a Data Scientist.

<figure align="center">
	<a href="/images/jd-classifier/TorandoChart_TermSensitivity_BothRoles.png">
    <img src="/images/jd-classifier/TorandoChart_TermSensitivity_BothRoles.png" style="width:50% !important;"></a>
    <figcaption>   Click image to enlarge</figcaption>
</figure>

Surveying the top terms for Data Scientist, results in a collection of words that are more technical in nature. Some of the top terms are: *machine learning*, *platform*, *algorithms*, *models*, *Java*, *programming*, *development* (see chart below). Because data science is more of a mix of a statistics and a computer science, these terms are not surprising at all. 

<figure align="center">
	<a href="/images/jd-classifier/TorandoChart_TermSensitivity_DataScientist.png">
    <img src="/images/jd-classifier/TorandoChart_TermSensitivity_DataScientist.png" style="width:50% !important;"></a>
    <figcaption>Click image to enlarge</figcaption>
</figure>

For Data Analysts, the key words tend to focus more on information dissemination, whether it be through through verbal or written form: *reports*, *reporting*, *dashboards*, *communication*, *verbal*. Data retrieval and organization is another theme that comes up: *excel*, *strong SQL*, *SQL skills*, *trends*.

<figure align="center">
	<a href="/images/jd-classifier/TorandoChart_TermSensitivity_Analyst.png">
    <img src="/images/jd-classifier/TorandoChart_TermSensitivity_Analyst.png" style="width:50% !important;"></a>
    <figcaption>Click image to enlarge</figcaption>
</figure>

## Final Thoughts
Whether the above solidified what you had previously perceived about the two roles or whether it was new information, the goal was to answer this common question from an employers perspective and hopefully in an automated way.

## Limitations and Next Steps
I have merely scratched the surface with this project and am excited to dig deeper to see how I can make the model more robust and insightful. For one, I would like to isolate terms based on the location or heading they are under in order to understand their level of importance for a given role. Furthermore, I'd like to collect a larger sample size and split out my data into junior and senior roles. 

To learn more about this project and stay updated about the progress, please feel free to check out [my github repo](https://github.com/pleonova/jd-classifier).


