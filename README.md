# Econometrics-R-Introduction
Hello there! If you are reading this, chances are you are starting your undergraduate course in econometrics. I created this as a high level overview for implimenting R into your econometric models and studies. This guide was specifically designed for students at Drury University taking ECON 375, but generally should have a good overview for what to expect and know whenever you take any econometrics undergraduate course. This is best assisted with the textbook "Using R for Introductory Econometrics" by Florian Heiss. Its about $27 on Amazon and I highly recommend it if you are starting out. However, hopefully I have done a good enough job here that you do not need this. If you have any further more specific questions or believe another topic should be added to this page, please email me at kschertzer@drury.edu. 

Attached you will find a sample dataset to work with as you learn. This is the same one that is going to be referenced in the code, so if you would like to follow along I recommend downloading it. I am going to have a section in here that covers where to find datasets and what to look for, so if you don't want to use this you will have options down there. 

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

If you are taking this course at Drury University, as of writing this you have access to ChatGPT for code help. What I recommend doing is having it write basic code and then you manipulate it from there. ChatGPT in my experience has been better about explaining what certain error codes mean, and not the best at fixing and rewriting the code. In the past it has caused more issues than it has fixed... With that being said, its improving every day and by Spring 2025 it may be way better and more capable. Do whatever feels right to you, but I would try to avoid having it do every part of it for you because chances are it won't be able to. 

The final note that I will give before I get into the details is that this is written assuming that you have a research paper to write. There are a lot of topics within here that are specific to that, so if you are learning on your own it may be harder to follow along without needing to write one. My personal recommendation is that you pick a dataset and try to formulate the research plan without actually writing the paper. Choose a topic, create a hypothesis, do the analysis, but background information isn't necessary here. 

## Basic Statistical Topics
It is important to begin at the very basics. To review, we remember that we have 
1. **Mean** - Average of all of the observations
2. Median - The middle value of all of the observations
3. Mode - The observation that is obtained the most
4. Variance - Average of the squared differences from the mean
5. Standard Deviation - The square root of the variance, indicates the dispertion of the data

Most of these will fall within the Normal Distribution, which you may remember as the classic bell shaped graph that you saw in your introduction to statistics class. This is what you will be dealing with most of the time. It is important to remember that in order for data to be considered 'normally distributed' it must have thirty or more observations. Luckily, virtually all datasets that you will be able to use are well over that so you will not have to worry too much about it. It is also important to be aware of a t-distribution as well as the chi-squared distributions, but these are not important at the introductory level.

You also will be dealing with hypothesis testing. Remember that these are defined as the Null and Alternative Hypotheses. They can be denoted as 

$$H_0 = Null$$

$$H_a = Alternative$$

The alternative hypothesis is interchangably written as H1 or Ha, your professor may have a preference but notation wise they are the same. For the rest of this page I will be using Ha, but please know that it means the same. 

The null hypothesis in the context of econometric modeling means that there was no effect in your Y and Beta1 variables. Your alternative will be the opposite where there will be an effect on Y with your Beta1 variable. Ultimately, you want your alternative hypothesis to be true. It is important to note here (and you may rememnber this from introduction to statistics), but we do not say "we accept the null hypothesis". There is two ways that we can phrase this 
1. We reject the null hypothesis - The alternative hypothesis is true
2. We **fail** to reject the null hypothesis - the null hypothesis is true

Again, for a basic econometric model we are generally going to aim to reject the null hypothesis, as no matter what we want some result in one way or another.

While we do aim to see some effect of a variable, it is **not** necessarily a bad thing to have to fail to reject and find no change. In the context of research, anything and everything is valuable. Sometimes, there being no effect is good, and can contribute to the greater knowledge of the topic equally the same as there being an effect. To summarize, theres really no right or wrong answer, results are results, don't aim to get one thing or another just aim to get **information**.

While this is pretty much the majoriy of the statistical knowledge needed to learn the rest, I **highly** recommend reviewing statistics at a high level before you get too far into the course. The more comfortable you are at statistics the easier this will be, as regression analysis is built off of mathematical and statistical theory. However, again, you really don't need to remember more than this. 

-----------------------------WORK IN PROGRESS --------------------------------------------

##Variable Types
When looking at your data you are going to be dealing with different types of variables, its important that you know these variables. It'll help you during your analysis later on if you know how these work right now. This will also make your data manipulation go a lot smoother in the long run.
1. Continuous variables - These are variables that can hold any value in a given range. A basic example of this is things like income, price, height, etc.
2. Discrete variables - these take specific values and cannot be between these given points, examples of this are number of children, number of cars, number of people in a classroom, etc.
3. Nominal variables





















