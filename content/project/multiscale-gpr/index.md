---
title: Multiscale Gaussian Process Regression
summary: Investigating weighted mix-ture of GPs method for handling multiscale features.
tags:
- Bayesian Learning
date: "2020-08-17T19:02:09-04:00"
math: true

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Weighted Mixture of GPs
  focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
url_code: ""
url_pdf: "files/6_435_Project_Final_Report.pdf"
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

In this project, I focus on modeling data which exhibit multiple correlation length-scales (multiscale) using different Gaussian Process Regression (GPR) models. Such data is relevant to physical processes where a cascade of interactions happens at different scales; for example, ocean flows where micro-turbulence happens at $\mathcal{O}$(1cm) to geostrophic eddies at $\mathcal{O}$(1000km).

Inspired by the Gaussian Mixture Model (GMM) based Kalman filters, I start with a weighted mixture of GPs for the prior, and then derived a closed-form solution for the posterior weights as well as for the mean and covariance function for each mixture model, which I will refer to as the \textit{weighted mixture of GPs} method. In this project, I compare the performance of some of these methods GP --- ARD kernel, Gibbs kernel, additive model and weighted mixture of GPs--- using synthetic 1-dimensional and 2-dimensional data. I compare  computational costs, and lastly, perform regression using actual data for daily fish catch in the Lakshadweep islands of India and a sea-surface-temperature (SST) satellite measurement near the east coast of the US.
