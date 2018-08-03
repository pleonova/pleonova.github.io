---
title: "AB Testing Playbook: Proportion"
date: 2018-08-03
tags: [ab testing, data science, statistics, python]
excerpt: "Data Science, AB Testing, Python"
---

# How to set up and evaluate an AB test?

So you need to run an A/B test and you need to figure out how many users you need in order to have valid results. What does "valid" results even mean? How do you decide what is the proper test to use to evaluate your results? 

In the following jupyter notebook, I go into how to run an AB Test from start to finish. I've highlighted which cells you need/might want to edit so that you can just step through the notebook without having to modify the majority. Think of it as a step by step guide or a template that you can plug in your own data.

This notebook focuses on how to both set up a proper test and evaluate it if your KPI is binomial (aka a proportion).

To view the jupyter notebook, please go [here](https://github.com/pleonova/ab-testing) 