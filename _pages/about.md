---
layout: about
title: about
permalink: /
subtitle: 

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  address: Universitetsparken 1, 2100 København Ø

news: false  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---

I am [Satyasaran Changdar](https://di.ku.dk/english/staff/vip/?pure=en/persons/723168), Postdoc in Machine Learning, [University of Copenhagen](https://www.ku.dk/english/) under the Supervisons of [Dr. Erik Bjørnager Dam](https://di.ku.dk/english/staff/?pure=en/persons/93620), Professor, [Department of Computer Science](https://di.ku.dk/english/), University of Copenhagen and [Dr. Kristian Thorup-Kristensen](https://plen.ku.dk/english/employees/?pure=en/persons/143157)
Professor, [Department of Plant and Environmental Sciences](https://plen.ku.dk/english/), University of Copenhagen, Denmark
 and completed my Ph.D. in applied mathematics in 2019 at [University of Calcutta](https://www.caluniv.ac.in), master of technology in computer applications from [Indian Institute of Technology, Delhi](https://home.iitd.ac.in), India in 2008 and masters in mathematics at [Indian Institute of Technology, Bombay](www.iitb.ac.in), India in 2005. 
Before joining Postdoc, I was working as an associate professor in [Institute of engineering and Management](https://iem.edu.in), Kolkata, India.

I specialize in Machine Learning, Deep Learning, Physics-informed Machine Learning, and Data-driven Scientific Computing. I have been actively involved in the development of machine learning methods that extract patterns from multimodal agriculture data in crop science from [RadiMax](https://cropinnovation.dk/some-of-the-projects/radimax/) in  [RadiBooster project](https://plen.ku.dk/english/research/crop_sciences/cpps/radibooster/). 

I have been collaborating with my PhD supervisor [Dr. Soumen De](https://scholar.google.co.in/citations?user=ZwIi7oUAAAAJ&hl=en) and supervising Phd Students [Bivas Bhaumik](https://scholar.google.com/citations?user=FfG_kKQAAAAJ&hl=en&authuser=3) and [Susmita Saha](https://www.researchgate.net/profile/Susmita-Saha-16) in University of Calcutta, India.

...

# Research Projects

## Radimax: Project 1:  Machine Learning for understanding plant root function [Paper Link:](https://doi.org/10.1007/s11104-023-06253-7)
[code link](https://github.com/satyasaran/CropML.git)

This project investigates the relationship between root distribution and resource uptake in crops using machine learning techniques. The study utilizes the RadiMax semi-field root-screening facility to phenotype winter wheat genotypes for root growth. Square root of planar root length [CNN, Deep learning was used to extract the root length from sub-soil images] density (Sqrt_pRLD) measurements are collected at different soil depths, and their correlation with deep soil nitrogen uptake and drought resilience potential is explored using machine learning models. The results demonstrate the importance of deep rooting for water and nitrogen uptake in crops.
### Results
Here are some images showcasing the results:

<div class="project-images">
    <img src="/assets/img/Fig2.jpeg" alt="Result 1" style="width: 400px;">
    <img src="/assets/img/Fig5a.jpeg" alt="Result 2" style="width: 400px;">
    <img src="/assets/img/Fig3a.jpeg" alt="Result 3" style="width: 400px;">
    <img src="/assets/img/Fig6a_left.jpeg" alt="Result 3" style="width: 400px;">
</div>


## Radimax: Project 2: Deep Learning for sub-soil Image analysis to investigate deep root function 

In Project 1, our objective was to employ deep learning techniques to analyze sub-soil images and investigate the function of deep roots in plant physiology. Specifically, we utilized transfer learning with the ResNet50 architecture to develop regression and classification models for root length estimation and root function investigation.


### Results

Here are some images showcasing the results:

<div class="project-images">
    <img src="/assets/img/grad1.png" alt="Result 1" style="width: 500px;">
    <img src="/assets/img/grad2.png" alt="Result 2" style="width: 500px;">
    <img src="/assets/img/grad3.png" alt="Result 3" style="width: 500px;">
</div>



## Project 3: Solving Non-liner Blood flow using Physics-informed Neural network
[Paper link](https://doi.org/10.1016/j.matcom.2023.10.011)

This work introduces a Python implementation of solution of non-liner PDEs arising in the process of arterial blood flow using DeepXDE. The proposed deep learning approach analyzes perturbations in arterial blood flow, with a focus on pressure and radius variations. The research develops a mathematical model for simulating viscoelastic arterial flow, incorporating long wavelength and large Reynolds number assumptions. Leveraging the reductive perturbation method, the study derives nonlinear evolutionary equations for medium resistance, elastic properties, and wall viscosity. By employing state-of-the-art physics-informed deep neural networks, trained via automatic differentiation, the implementation efficiently solves these equations. Bayesian Hyperparameter Optimization identifies the optimal neural network architecture, providing an efficient and accurate alternative to numerical methods for medical machine learning applications.

### Results

Here are some images showcasing the results:
[Image sources: published Paper link](https://doi.org/10.1016/j.matcom.2023.10.011)
<div class="project-images">
    <img src="/assets/img/pinn.jpg" alt="Result 1" style="width: 500px;">
    <img src="/assets/img/loss.jpg" alt="Result 2" style="width: 500px;">
    <img src="/assets/img/sol1.jpg" alt="Result 3" style="width: 500px;">
    <img src="/assets/img/sol2.jpg" alt="Result 3" style="width: 500px;">
    <img src="/assets/img/sol3.jpg" alt="Result 3" style="width: 500px;">

</div>



