---
title: Physics-Inspired Machine Learning for PDEs
summary: Implementation  of  Machine Learning  algorithms  for  solving  nonlinear  partial  differential equations, in a hybrid framework.
tags:
- Deep Learning
date: "2020-08-17T19:02:09-04:00"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: The implemented LSTM-RNN architecture coupledwith the evolution equations
  focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
url_code: ""
url_pdf: "files/ML_Project_Final_Paper.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example

# Optional header image (relative to `static/img/` folder).
# header:
#   caption: "Weighted Mixture of GPs"
#   image: "GMM_indiv_post.png"
---

This  work  studies  the  implementation  of  Machine Learning  algorithms  for  solving  nonlinear  partial  differential equations, in a hybrid framework. Specifically, Recurrent  Neural  Networks  (RNN)  and  Convolutional Neural  Networks  (CNN)  are  used  to  reduce  the  high computational costs involved in solving such problems. We  do  not  use  Neural  Nets  to  perform  predictions  for next  time-steps  but  to  replace  the  computationally  demanding parts of the system.  We implement this hybrid approach for the study of the evolution of free-surface waves.  As a first test case, we study the propagation of a  wave  in  a  periodic  cell.   For  this  case  we  track  the conservation errors regarding the time evolution of theproblem.  Afterwards we model the reflection of a solitary wave on a vertical wall and compute the force acting on the wall. We also see the effect of varying hyper-parameters on the accuracy of prediction of our neuralnets,  and perform leading order FLOP count compar-isons.
