---
layout: post
title: "Recurring Brain Fails"
excerpt: A summary of a talk on how programming paradigms affect the way we approach problems.
category: computer-science
tags: ["computer-science"]
date: 2016-01-19
---
I recently joined a meetup group called Papers we Love, that aims to get people together to talk about interesting papers and research problems. After much reluctance and grumbling about poor life decisions, I finally found myself at a session on a Sunday evening. The topic was a discussion of the Recurring Rainfall problem from a pedagogical perspective, by Dr. Shriram Krishnamuthi, a Professor of Computer Science from Brown University, who has spent a considerable number of years trying to understand and improve the way programming is taught to undergraduates.

So the premise of Soloway's Recurring Rainfall problem is simply this: Design a program called rainfall that consumes a list of numbers representing daily rainfall amounts as entered by a user. Produce the average of the non-negative values in the list up to the first -999 (if it shows up).

This seemingly trivial problem has the infamous distinction of over 70% of beginning level programmers getting it wrong - a result that was reproduced over decades of experiments. This has been usually attributed to the fact that it requires the programmer to do multiple subtasks, all of which together become difficult for a first time programmer to handle. 

The entire talk is put up <a href="https://www.youtube.com/watch?v=O-F-IXQGtjs"><u>here</u></a>, and <a href="http://www.cs.tufts.edu/~nr/cs257/archive/kathi-fisler/icer14.pdf"><u>this</u></a> is the paper on the topic. I found the talk  really enlightening for several reasons that I'll go into, not the least of which is the fact that such solid research is being devoted to the study of how programming is taught and learnt. Since programming is touted to become an indispensable skill in the years to come, such research is likely to be well worth the effort.

One part of the debate revolved around the difference in the ways that imperative and functional programmers approach problems. Over a set of controlled experiments on entering freshmen  at Brown University, it was first inferred that functional programmers preferred cleaner, modular solutions with separation of concerns as compared to imperative programmers that preferred the 'single loop' approach, often leading to more convoluted code that was consquently more buggy. Students who had been exposed only to imperative paradigms were found to passionately avoid operations that created intermediate data structures (possibly out of concern for memory efficiency), while Haskell programmers prefered decomposing problems and often created  data structures to store results of intermediate cleaning or parsing operations.

This inference was turned on its head however, when library functions were brought into the mix. Then, OO progammers were more than willing to use these functions, unmindful of the data structures they used internally, while functional programmers willingly sacrificed separation of concerns for functions that got the job done faster. I've personally often subscribed to such behavior in the past, with some misplaced notion of library implementations being 'super-optimized' and okay to use in nearly all cases, though this is often far from the truth.

Another interesting suggestion was that programmers write tests before coding up the algorithm, similar to writing examples before solving math problems. By observing the structure of the output, it is possible to discover the structure in the problem and come up with efficient ways to decompose it. Though an interesting idea, I once again felt, based on my personal example, that the tests I wrote were simply one standard test and all the possible edge cases. In order to discover structure, I feel that we, hardened imperative programmers, will need to start writing less 'imperative' tests as well!