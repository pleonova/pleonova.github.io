---
title: "What is the difference between a Data Scientist and a Data Analyst?"
date: 2018-08-21
tags: [Classification, Python, Naive Bayes]
excerpt: "A model that predicts the role from just the job description."
mathjax: true
---

## Objective
What can we learn from looking at job descriptions for these two roles? What keywords are found in both and which are more unique and help distinguish the roles?

## Background
I extracted the words and phrases from job descriptions of the big tech companies in Silicon Valley and built a supervised model to see if it could predict, from just the description, whether the role was for a data scientist or data analyst.  

## Summary
I ended up training a Multinomial Naives Bayes model to predict the job titles with an **accuracy of 76%**. Unsurprisingly, the top key words/phrases for data scientist were: “machine learning”, “models”, "algorithms" while that for data analysts were: “reports”, “dashboards”, and “excel”. 

## Takeaways
**Examining the results that my model classified in correctly actually gives insight into employers and their expectations.**

There are several reasons why a company might choose to display a title where the description does not match the role. Lyft, for example, on their blog, wrote the following article [What's in a name?](https://eng.lyft.com/whats-in-a-name-ce42f419d16c), where they explained that they strategically chose to change the title of a data analyst to a data scientist to retain talent (in my model, this role comes up as a false positive). However, instead of encompassing both roles in one title, they updated that of data scientist to research scientist. Others have done it to attract talent and get a pool of applicants that are simply drawn to the [Sexist Job of the 21st Century](https://hbr.org/2012/10/data-scientist-the-sexiest-job-of-the-21st-century), as initially proclaimed by Harvard Business Review. While others have done it to attract more skilled workers.

I am curious if other companies will follow this example and broaden the definition of a data scientist. Will more companies use these two terms interchangeably or create new terminology like research scientist? As a follow up to these questions, I'd like to eventually (A) re-test my model on a set of new job descriptions and (B) build an unsupervised clustering model to see which jobs get grouped and whether new titles emerge. 

**Frequent terms establish the baseline knowledge expected in both roles, while frequent but unique terms per role highlight key differences.**
 
It is no surprise that *sql* and *analysis* show up frequently in both postings. What is interesting, however, is that *statistics* shows up in both. Context is very important; the words that show up surrounding this term provide additional information about the level of expertise required. Upon further inspection, it looks like this term frequently shows up alongside a list of other quantitative degrees, for both roles, so it is less surprising than it was at initial glance. Another term that appears frequently for both is *python*. The frequency of which this word shows up for Data Scientist roles is, however, significantly higher than the times it appears in data analyst JDs. Almost 90% of the data science roles contain the key term, while only 60% of the data analyst JDs have it, indicating that python is an expected skill for a data scientist.

<img src="https://github.com/pleonova/jd-classifier/blob/master/Images/TorandoChart_TermSensitivity_BothRoles.png" width="400" align="center">

Surveying the top terms for just a Data Scientist, results in a collection of words that are more technical in nature. Some of the top terms are: *machine learning*, *platform*, *algorithms*, *models*, *java*, *programming*, *development*. Because data science is more of a mix of a statistician and a computer scientist, these terms are not surprising at all. 

<img src="https://github.com/pleonova/jd-classifier/blob/master/Images/TorandoChart_TermSensitivity_DataScientist.png" width="400"> <img src="https://github.com/pleonova/jd-classifier/blob/master/Images/TorandoChart_TermSensitivity_Analyst.png" width="400" align="right">

## Next Steps
I have merely scratched the surface with this project and am excited to dig deeper to see how I can make the model more robust and insightful. For one, I would like to isolate terms based on the location or heading they are under in order to understand their level of importance for a given role. Furthermore, I'd like to collect a larger sample size and split out my data into junior and senior roles. 

To learn more about this project and stay updated about the progress, please feel free to checkout [my github repo](https://github.com/pleonova/jd-classifier).




there are nearly 

There seems to be a bit more uniformity for data scientists, based on the percentage of common, but unique terms that show up. Looking at terms that show up in at least 30% of JDs, there is more variety of terms for data analysts (182 terms versus 158).




, however this terms does show up slightly more in data science positions. It is also important to understand the depth of statistics knowledge required might be different is worth examining within the context of the JD. Upon further investigation


Obviously, the top key terms will 

but you can't overlook the skills that are listed in both. 


to narrow down which areas to focus on depending on which job one wants to land while the key words that overlap could help someone prepare for a career transition. * 

focus in on where to spend 

* As interesting at the top key words are, the overlap between they two roles is also insightful”
* As … are perhaps more actionable if someone is looking to transition. 


To learn more about this project, please feel free to checkout [my github repo](https://github.com/pleonova/jd-classifier).