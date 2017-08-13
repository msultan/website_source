+++
abstract ="Efficient sampling of protein dynamics"
authors = ["Mohammad M Sultan", "Vijay S Pande"]
date = "2017-04-10"
image = ""
image_preview = ""
math = true
publication = "Journal of Chemical theory and Computation"
publication_short = ""
selected = true
title = "tICA-Metadynamics: Accelerating Metadynamics by Using Kinetically Selected Collective Variables."
url_code = ""
url_dataset = ""
url_pdf = "http://pubs.acs.org/doi/pdf/10.1021/acs.jctc.7b00182"
url_project = ""
url_slides = ""
url_video = ""

#[[url_custom]]
#name = ""
#url = ""

+++

Metadynamics is a powerful enhanced molecular
dynamics sampling method that accelerates simulations by
adding history-dependent multidimensional Gaussians along
selective collective variables (CVs). In practice, choosing a
small number of slow CVs remains challenging due to the
inherent high dimensionality of biophysical systems. Here we
show that time-structure based independent component
analysis (tICA), a recent advance in Markov state model
literature, can be used to identify a set of variationally optimal
slow coordinates for use as CVs for Metadynamics. We show
that linear and nonlinear tICA-Metadynamics can complement existing MD studies by explicitly sampling the system’s slowest
modes and can even drive transitions along the slowest modes even when no such transitions are observed in unbiased
simulations.