---
layout: post
title: "Why Is Computer Vision Hard?"
excerpt: "A brief overview of how far we've come and what lies ahead."
category: Computer Science
tags: [research, computer-vision, thoughts]
date: 2015-07-02
---
Nearly all fields of computer science have made leaps and bounds in the past few decades. We've created personal
computers that can process data orders of magnitude larger than the fastest supercomputers of just a few years ago.
The internet has scaled up to become the all knowing, all pervasive oracle it is today. We've built cars that drive
themselves, created immersive augmented reality experiences that blur the lines between real and virtual, and even
tried our hand at Terminator vision.

With such dazzling progress, it's quite relevant to ask why how far along we've come in machine vision, and to be fair
the answer is - an impressive amount. Right from low level image de-noising and compression techniques to higher level
semantic parsing and the ultimate aim of 'scene understanding', researchers have made several breakthroughs to get us
to where we are today.

In an illuminating talk on the <a href="https://www.youtube.com/watch?v=ylVsqXzlJqA">history of computer vision</a> Stanford's Fei Fei Li admits how today's visual systems, though massive improvements over their predecessors, still cannot perform the visual processing done by a year-old
baby. At this point, it's essential we understand and appreciate what makes vision as complex as it is.

In his now famous <a href="https://www.google.co.in/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=0CCkQtwIwAQ&url=http%3A%2F%2Fwww.ted.com%2Ftalks%2Fbeau_lotto_optical_illusions_show_how_we_see%3Flanguage%3Den&ei=RKNYVdTbIajhywPHjICgBw&usg=AFQjCNEjSCcoBp8PEi619j58MeFudgAsqg&sig2=bZ3DJ4WqphNK9lo6ceKQJg&bvm=bv.93564037,d.bGQ">
TED talk</a>, Beau Lotto talks about the subtle complexities of human vision. He proves how our vision is context
sensitive and statistical through live counter-intuitive experiments, to the visible astonishment of the audience.
Our perception of something as seemingly simple as a object's color thus depends on factors ranging from the
intensities of its neighboring regions, the surrounding illumination and our evolutionary conditioning over thousands
of years.

The task of replicating such a complex system is naturally riddled with difficulties - to start with, there are
several different kinds of visual processing in the human eye and brain, and computer vision needs to determine the
best approach to mimic. Even then, the very objective of replicating our complex visual cognition in machines is
truly daunting. Our vision is a beautifully intricate neural network that has evolved over several millennia to see
the world in a manner most useful to our survival, and is still not understood completely by neuroscience.

Additionally, computer vision is extremely mathematically involved; some would argue that it is entirely mathematics.
Vision makes use of mathematics spanning the breadth of linear algebra, multivariable calculus and probability and
statistics, which in my experience makes it less accessible to the average CS grad.

But despite these challenges, we're getting there. It's only a matter of time before Dr. Li stands corrected.
