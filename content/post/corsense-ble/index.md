+++
title = "Real-Time HRV Collection using CorSEnse"
subtitle = ""
date = 2024-04-06T00:00:00Z
draft = false  # Display this post? (true/false)

authors = ["admin"]

tags = ["Heart-Rate", "Bluetooth", "corsense", "HRV","filtering"]
summary = "An interface for reading and filtering HR and HRV data from corSense device by EliteHRV in real-time using Bluetooth Low Energy (BLE)."

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references 
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
# projects = ["internal-project"]

+++

## Artefact Detection
Artefact detection is based on a moving window of median RR (window size = 10).

<img class="special-img-class" style="width:70%" src="RR.gif" />
