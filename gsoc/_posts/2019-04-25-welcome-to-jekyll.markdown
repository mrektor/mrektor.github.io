---
layout: post
title:  "GSoC for OpenAstronomy"
date:   2019-04-25 12:29:15 +0200
categories: general
---
My intent with this site is to allow anyobody who might be interested in my works to follow my progresses.

I’ve heard about OpenAstronomy and the GSoC thanks to my master thesis supervisor [rlopezcoto](https://github.com/rlopezcoto). I then proposed to work on the project of reconstructing the energy and direction of IACT events with deep learning and to integrates such models in CTLearn, an open-source python library.

My experience applying these method comes from the work done in my master thesis where to perform a full reconstruction of data from the currently operating MAGIC telescopes. To do that I started from the calibrated data which I interpolated using scipy in order to make the data computable from the keras deep learning framework. These data was used for solving the *regression* problem of _energy_ and _direction_ reconstruction by fitting convolutional neural networks architectures and optimizing them with innovative techniques taken from the recent literature. The full repository with all the code developed for this task is [here](https://github.com/mrektor/CNN4MAGIC).

The interpolation step is already solved in CTLearn by the DL1-data-handler so I am proposing to implement some of the regression routines using neural networks exploiting multi-task learning (MTL).

