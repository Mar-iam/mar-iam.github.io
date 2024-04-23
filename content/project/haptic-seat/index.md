+++
title = "Haptic Seat in 3D Driving Simulation"
date = 2019-04-05T02:44:40+01:00
draft = false

# Tags: can be used for filtering projects.
tags = ["virtual-reality","haptic"]

# Project summary to display on homepage.
summary = ""

# Slides (optional).
#   Associate this page with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references 
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides = ""

# Optional external URL for project (replaces project detail page).
external_link = ""

# Links (optional).
url_pdf = ""
url_code = ""
url_dataset = ""
url_slides = ""
url_video = ""
url_poster = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
# links = [{icon_pack = "fab", icon="twitter", name="Follow", url = "https://twitter.com"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
[image]
# Caption (optional)
#  caption = ""
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""
  preview_only = true

+++

# Overview
In the undergraduate senior project, we developed a 3D driving simulation in an immersive environment, that is projected on CAVE and HMD display systems, using [Vizard VR Toolkit](https://www.worldviz.com/vizard). The simulation was integrated with a set of vibrators mounted in the back seat to deliver navigational information to the driver. 

## High-level architecture
<img class="special-img-class" style="width:70%" src="hla.png" />

A set of 10 vibrators were distributed in the back seat based on several experiments to determine the appropriate intensity of vibration, the pattern, and the minimum distinguishable distance. They have been arranged as 4, 2, 4 vibrators in each column. The first two rows corresponded to the _"straight"_ signal, whereas the first and last columns indicated the _"left"_ and _"right"_ signals respectively.

## Evaluation
A predefined scenario was designed in the 3D driving environment to navigate the drivers to a certain destination. The overall effectiveness of the vibrotactile seat was measured based on the response time and the number of correct responses as compared with audio-directional feedback. The response time was measured between the time the navigational aid was triggered and the time in which the user responded and took action. 

Further details about the design of the tactile seat and the study analyses are discussed in the following papers: