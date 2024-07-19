# Econometrics-R-Introduction
Hello there! If you are reading this, chances are you are starting your undergraduate course in econometrics. I created this as a high level overview for implimenting R into your econometric models and studies. This guide was specifically designed for students at Drury University taking ECON 375, but generally should have a good overview for what to expect and know whenever you take any econometrics undergraduate course. This is best assisted with the textbook "Using R for Introductory Econometrics" by Florian Heiss. Its about $27 on Amazon and I highly recommend it if you are starting out. However, hopefully I have done a good enough job here that you do not need this. If you have any further more specific questions or believe another topic should be added to this page, please email me at kschertzer@drury.edu. 

## Table of Contents
1. [Introduction](#Introduction)
2. Basic Statistical Concepts
3. Variable Types
4. Selecting a research topic
5. Downloading and Installing RStudio 
6. Selecting Your Data
7. Merging Data 
8. Cleaning Your Data
9. Manipulating Your Data
10. Simple Linear Regression
11. Multiple Linear Regression
12. Assumptions of the Classical Linear Regression Model
13. Model Diagnostics and Remedial Measures
14. Intermediate Regression Topics
15. Time Series Analysis
16. Forecasting Techniques
17. Advanced Regression Topics
18. Help/Error Guide

## Introduction
Contrary to popular belief, economics is less of a business degree than it is a statistics degree. The foundation of all economic theory lies within statistics, and more specifically research. Most economists who successfully are able to make their way into the field of economics will tell you that most of their workload consists of doing math and coding, with writing taking a strong third place. If you have made it this far in your degree, chances are you have at least a little bit of curiosity in you about how the world works and functions. 

Econometrics is the core of economic research past the undergraduate levels. It lies in an applied area of statistics and mathematical study that crosses over with business topics. The goal by the end of this course is that you have a high level understanding of the topic. I want to emphasize, that you by no means need a large statistics or math background to successfully complete this course. While having that background and understanding would be helpful, it is by no means necessary. You also do not need any more than a very basic understanding of coding in order to accomplish this. 

This will be discussed later in the page, but it should be known that this will not specifically teach you how to calculate these models by hand. If you are looking for a guide for that, it is currently a WIP and should be up by January 2025. However, this guide will teach you how to obtain the models through the use of R as well as how to accurately interpret the models. 

If you are having code issues, I recommend skipping straight to the Help/Error Guide at the bottom of this page. It has a better guide on where to go and what to do when you run into error messages. Unfortunatley, R isn't as user friendly as other coding languages like Stata (and also doesn't have nearly as good help options when errors do occur)

The final note that I will give before I get into the details is that this is written assuming that you have a research paper to write. There are a lot of topics within here that are specific to that, so if you are learning on your own it may be harder to follow along without needing to write one. My personal recommendation is that you pick a dataset and try to formulate the research plan without actually writing the paper. Choose a topic, create a hypothesis, do the analysis, but background information isn't necessary here. 

## Basic Statistical Topics
It is important to begin at the very basics. To review, we remember that we have 
1. **Mean** - Average of all of the observations
2. Median - The middle value of all of the observations
3. Mode - The observation that is obtained the most
4. Variance - Average of the squared differences from the mean
5. Standard Deviation - The square root of the variance, indicates the dispertion of the data

Most of these will fall within the Normal Distribution, which you may remember as the classic bell shaped graph that you saw in your introduction to statistics class. This is what you will be dealing with most of the time. It is important to remember that in order for data to be considered 'normally distributed' it must have thirty or more observations. Luckily, virtually all datasets that you will be able to use are well over that so you will not have to worry too much about it. It is also important to be aware of a t-distribution as well as the chi-squared distributions, but these are not important at the introductory level.


---------------------EVERYTHING BELOW THIS IS A WIP--------------------------------------

You also will be dealing with hypothesis testing. Remember that these are defined as the Null and Alternative Hypotheses. They can be denoted as 

$$H_0 = Null$$

$$H_a = Alternative$$

The alternative hypothesis is interchangably written as H1 or Ha, your professor may have a preference but notation wise they are the same. For the rest of this page I will be using Ha, but please know that it means the same. 





















