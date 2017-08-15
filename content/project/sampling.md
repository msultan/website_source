+++
# Date this page was created.
date = "2016-11-28"

# Project title.
title = "Advanced Sampling"

# Project summary to display on homepage.
summary = "Faster sampling via Markov decision processes(MDP) and Reinforcement-Learning."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "rl.png"

# Optional image to display on project detail page (relative to `static/img/` folder).
image = "tica_meta.gif"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["machine-learning","sampling"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

+++

I have been interested in using MSM to extend the capability of MD simulations. The fundamental question I am
interested in answering if whether we can reduce the computational complexity of a new simulation by leveraging
information from the current MSM. The new simulation could be a new sequence, a new physics model or perhaps
some post translational modification. To that end, I am borrowing ideas from Reinforcement-Learning and Markov decision
processes.

Recently, I showed over [a](http://pubs.acs.org/doi/abs/10.1021/acs.jctc.7b00182) [series](http://www.biorxiv.org/content/early/2017/07/02/158592)
 of papers that the [tICA](http://msmbuilder.org/3.8.0/decomposition.html#tica) algorithm can be used to
form better CV than human intuition in enhanced sampling algorithms such as Metadynamics/Umbrella sampling. This is