+++
title = "Data Visualisation in Large Displays"
date = 2019-04-05T02:45:33+01:00
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["visualization"]

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
#  # Caption (optional)
#  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""
  preview_only = true

+++
# Overview
This work was part of my master's project at Imperial College London under the supervision of Dr. [David Birch](https://scholar.google.co.uk/citations?hl=en&user=0w0rO70AAAAJ). The primary aim was to integrate a scientific visualisation tool, ParaView, with the Data Observatory (DO) at the [Data Science Insititute](https://www.imperial.ac.uk/data-science/data-observatory/) to foster data exploration. The DO is a large tiled-display system consisting of 64 screens providing a resolution of over 130 megapixels. 

{{< figure src="featured.jpg" title="A snapshot of the inner view of 3D brain model displayed in the DO" >}}

## Implementation
The main approach was to split the 3D model, displayed in ParaView, across 64 screens over a distributed clustered network. This was achieved by controlling the viewing camera for each screen and ensuring the alignment of the overall scene. Moreover, the [MPI protocol](https://en.wikipedia.org/wiki/Message_Passing_Interface) was used to distribute the data rendering and processing over multiple machines.

## Evaluation
The integration of ParaView with the DO provided a high-resolution visualisation of scientific models and enabled researchers to collaborate with each other. Therefore, the effectiveness of large display environment as compared with small screens was assessed in terms of evaluating the task performance and collaboration.

1. **Task Performance:**

    A mental rotation task was designed to evaluate the perceptual and cognitive performance of researchers in both environments. It is one of the popular tests that is mainly used to identify the ability to detect orientation change in 3D objects from two perspectives [^1]. Each participant was asked if the displayed models were the same or mirrored.
[^1]: R. N. Shepard and J. Metzler, “Mental Rotation of Three-Dimensional Objects,” Science, New Series, 1971. 

{{< figure src="mental.png" title="Mental rotation task in two cases: (1) The same (2) Mirrored" >}}

2. **Collaboration:**

    In the collaboration task, the participants were asked to work in pairs and search for hidden objects -represented as coloured arrows- injected inside a 3D brain model while discussing within a limited time. 

For both tests, the number of correct responses was measured to conduct quantitative analysis. The results showed a significant advantage of using the DO as compared with the typical desktop monitor in the accuracy of the mental rotation and collaborative search tasks.