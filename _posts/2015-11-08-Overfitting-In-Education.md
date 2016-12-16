---
layout: post
title: "Overfitting in Education"
excerpt: A critique of the Indian education system, inspired by Machine Learning.
category: computer-science
tags: ["computer-science", "education"]
date: 2015-11-08
---

The Indian education system receives a fair amount of flak for its focus on rote learning and its discouragement of independent thought. It's also riddled with issues ranging from inefficient bureacracies to politically motivated reservation and a shortage of funding. However, it's the issues with pedagogy that I'd like to address here, by (loosely) borrowing an analogy from the field of Machine Learning.

First off, the approach to designing syllabi is largely breadth-first. We study a staggering breadth of subjects right from elementary school, across math, science, social sciences, environmental studies, English and vernacular languages. Add a couple of vocational subjects in secondary school, and you see kids swamped with homework and bogged down by the weight on their shoulders. Each of these subjects typically has a massive syllabus that teachers constantly fret about finishing on schedule. Altogether, it's no wonder that we fail to really delve into topics with any respectable depth - there simply isn't any time.

But that's just the tip of the iceberg.

I believe the more pressing issue is that our educational training massively overfits young minds to the subject matter. Our tests generally ask questions right out of the training set of solved examples and classroom content, and the student with the highest prediction accuracy on the training set walks away the winner. Simply put, rote learners ace tests. Unfortunately, this pedagogy is rarely questioned due to a combination of lethargy and a misplaced confidence in our evaluation metrics -  but our accuracy metrics are all wrong!

<img class="blog_comic" src="images/CH_rote_learning.jpg" alt="Calvin on Rote Learning" / style="width:448px;height:194px;" />

As a result, Indian kids are underprepared to apply their learning right out of school. When it's something similar to something we've seen before, it's a breeze, but we struggle when faced with problems that requires us to <i>generalize our learning</i>, on questions that are 'application-oriented' or that require 'critical thinking'. And in today's globalized day and age, the claim of a difference in training data doesn't hold water anymore - we have access to the top literature on most subjects, on par with the subject matter at top universities globally. 

What I'm ultimately claiming is this: There's not much wrong with the content, it's the training that's going awry.

So how do we fix this?

Typically, overfitting is addressed by one of the following methods:

<ol>
<li> Increasing the size of the training set </li>
<li> Reducing the number of features </li>
<li> Regularizing the model </li>
</ol>
Now right off the bat we have to reject (1) a on purely humanitarian grounds - we already study copious amounts of subject matter, thankyouverymuch. Reducing the number of subjects is certainly a viable option, but sparks off a whole new debate about which subjects are less important and should be scrapped, and won't get us anywhere. So what we're left with is regularization.

In regularization, we add a 'regularization parameter' to try to keep the the model parameters small while still minimizing the cost function. The rationale is to obtain a 'simpler' model that is heuristically found to generalize better. Analogously, we can introduce simple thought exercises in the classroom that test a thorough grasp of fundamentals rather than mastery of every kind of solved example. Short tests or pop quizzes on unseen problems (that form our cross validation set)  can be used to figure out what areas need to be focused on more, and thus tweak the 'hyperparameters' of our training model to maximize performance on this validation set. More simply, a larger focus on developing critical reasoning skills can go a long way in fixing our overfitting issue.

Of course, we also need to address the problem with our testing. We can try and emulate the standard training-cross validation-test split approach to our subject matter and ensure the tests contain questions that the students haven't seen before, and are thus encouraged to think critically and approach them from the basics. Only then will the results be truly reflective of our understanding, and not our memory alone. And it'll be a small but sure step towards preparing us to actually apply what we learn at school.