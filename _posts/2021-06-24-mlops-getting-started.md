---
title: "My MLOps Journey - Getting Started"
date: 2021-06-24
tags: [MLOps, Deeplearning.ai, Machine Learning]
excerpt: "How I am approaching learning MLOps and what resources I started with."
mathjax: true
---

This is a somewhat lengthy post, but I wanted to provide you, the reader, with a bit more background about how I approach learning, specifically MLOps, in the hopes of either reducing the cold start problem of finding your first resource in the area or perhaps reducing some anxiety around the perceived linearity of learning and the importance of getting your feet wet, even if it means just dipping your toes in (my sad attempt at a metaphor of how it is better to try something, even if it is very small, rather than standing on the sidelines because you are afraid of jumping in headfirst - though, when it comes to swimming, sometimes the latter is actually easier - but I digress). 

Below, I’ve outlined three steps that I have been following and the resources I have found invaluable in my learning journey. 

# Step 1: Familiarize myself with the MLOps landscape
Finding a good starting learning resource to reference makes a whole lot of difference. However, this can take time as there are lots of resources and the first one may not always be a good fit, therefore I tend to jump around a bit in the beginning between different resources until I find something that I can sink my teeth into. My go to strategy to get a solid foundation in a topic is to audit online courses and read through O’Reilly textbooks, which I supplement with blog posts, tutorials and eventually papers. Sometimes I do the latter in order to get a better lay of the land.

Initially, in my Machine Learning Operations journey, I was following Goku Mohandas’ MLOps lessons as he was posting them. I came across his website madewithml.com before the pivot from an AI forum aggregator of sorts to a more MLOps focused course. There were certain topics I wanted to jump to that he hadn’t yet posted about, so I started looking around for additional resources (at time of writing, he has posted all the lessons and I would highly recommend this resource).

It wasn’t too much later that DeepLearning.ai announced their newest MLOps specialization. I had, for a brief period, however, actually taken a small pause from my initial MLOps goal while Goku uploaded the remaining lessons, to focus on NLP - another topic I was particularly interested in. *Thankfully* there is no shortage of material to learn in data science (I say that both sarcastically and enthusiastically). I had bookmarked a while back [Stanford’s CS 224: Natural Language Processing with Deep Learning](http://web.stanford.edu/class/cs224n/) and so started going through the material. I wanted to supplement the class with another one and also started taking Deeplearning.ai’s NLP courses, which is where I heard about the latest specialization launch. Andrew Ng was teaching the first course in the MLOPs series and since I am a big fan of his teaching style, which tends to focus on practical hands-on experience with just enough theory so you understand the formulas and tradeoffs at a high level, I was really excited about the course. At this point, I got back on track to my MLOps journey.

# Step 2: Get to coding as soon as possible
The labs in the first course [Introduction to Machine Learning in Production](https://www.coursera.org/learn/introduction-to-machine-learning-in-production?specialization=machine-learning-engineering-for-production-mlops) of the MLOps deeplearning.ai specialization were great as they focused on getting a model up and running and were super well documented. I pretty much immediately jumped to these after only an hour of watching the material so I could see how the course content was applied to a problem (I would highly recommend reading through and running the [Ungraded Lab Part 1 - Deploying a Machine Learning Model](https://github.com/https-deeplearning-ai/MLEP-public/blob/main/course1/week1-ungraded-lab/server.ipynb) notebook).

I also searched for additional tutorials to see what other approaches there were. I found this fantastic youtube tutorial by Mike Nemke: [Rapidly build & deploy an NLP / Machine Learning App with Poetry, FastAPI, Docker, Spacy & GCP](https://www.youtube.com/watch?v=Maj9v-Ev7-4) and the [accompanying blog post here](https://www.mktr.ai/building-and-deploying-an-ml-app-part-1/) and coded along with the step by step tutorial. I thought that it was very easy to follow along and provided just enough information about the various tools used that you knew how they fit into the overall picture. Since the video is a little older, a few dependencies needed to be handled differently, but otherwise you can get an NLP model up and running on the Google Cloud Platform within a few hours.

I’ll admit that I often have more questions after following these tutorials and go back to step 1 instead of 3. I can sometimes find myself going down a rabbit hole by trying to get a solid foundation in every topic/concept I encounter. At a certain point, once I have enough of the basics down however, I need to get to step 3. Inevitably, more questions will arise and it will become an even less linear of a learning process, the goal is however to get a version of my minimum viable product up and running, rather than just following along a tutorial.

I think trying to have every step in MLOps perfected/fully understood is futile (I think this is true for many topics in Data Science). In order for it to be more manageable, from a learning perspective, I think a more iterative approach is best. Get something to work, review reference material, add another part of the pipeline working, look up a new step, just keep further optimizing the steps, the key is do it in parts, so something is working, even if it is not the most optimal at first, afterall “Perfect is the enemy of good”. 

# Step 3: Apply what I have learned so far to my own problem
Once I get a few practical examples under my belt and am aware of a couple of different approaches, I try to fit my own problem into the solutions I’ve found. I don’t try to upend everything at once, but rather modify parts that will help me get closer to solving my problem. Here, I also try to simplify my own problem, perhaps reducing it to its absolute core, so that my model is not the most accurate but requires less computation and fewer steps. In this case, the goal isn’t a perfect model, but rather an MVP.

This is the most important step and where a lot of learning takes place. It’s also the hardest, but the most rewarding, if you keep at it. Getting practical hands-on experience is key and overcoming the hurdles that you will inevitably encounter will make you a better data scientist as those are the types of problems you’ll face on a day to day. 

## List of MLOps resources in this blogpost:
- [Andrew Ng: Deeplearning.ai’s Introduction to Machine Learning in Production](https://www.coursera.org/learn/introduction-to-machine-learning-in-production?specialization=machine-learning-engineering-for-production-mlops)
- [Mike Nemke: Rapidly build & deploy an NLP / Machine Learning App with Poetry, FastAPI, Docker, Spacy & GCP](https://www.youtube.com/watch?v=Maj9v-Ev7-4)
- [Goku Mohandas: Made with ML - MLOps course](www.madewithml.com)

Also, if there are any resources you have found invaluable in your journey, I would love to hear about them!
