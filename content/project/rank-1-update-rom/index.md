---
title: Active rank-1 updates to POD based reduced order models
summary: Investigation of a method for efficiently updating a reduced order model online, as new data becomes available corresponding to system changes.
tags:
- Reduced Order Modeling
date: "2020-08-17T19:02:09-04:00"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Reduced-Order-Modeling for 2-D advection-diffusion equation.
  focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
url_code: ""
url_pdf: "files/18_335_Report.pdf"
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

Simulating physical systems is often a computationally expensive task. Data driven reduced order models are typically applied in these situations and provide accurate and low cost evaluations of the system. In some cases, changes in resources or system state may cause such models to become unreliable and inaccurate in new domains. Costly reconstructions of the reduced order model at each system change can sacrifice the speed benefits of using a reduced order model. This project investigates a method for efficiently updating a reduced order model online, as new data becomes available corresponding to system changes. New data is incorporated as low rank updates to proper orthogonal decomposition (POD) basis and reduced operators that allow the reduced order model to adapt with the system domain. This dynamic approach is competitive in accuracy compared to rebuilding the method from scratch, but is able to significantly decrease time complexity. The method is demonstrated on the advection-diffusion equation and we show that after sufficient data has been incorporated, our dynamic reduced order model is able to converge to the accuracy of the true model by making efficient updates online.
