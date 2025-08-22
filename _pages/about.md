---
layout: about
title: about
permalink: /
subtitle: ""
profile:
  align: right
  image: assets/img/satyaku.jpeg
  image_circular: false
  address: University of Copenhagen, Denmark
news: false
selected_papers: false
social: true
---

I am [Satyasaran Changdar](https://di.ku.dk/english/staff/vip/?pure=en/persons/723168), Assistant Professor, working in the areas of sustainable food process modeling and new food formulation, Ingredient and Dairy Technology, Department of [Food Science](https://food.ku.dk/english/) at the [University of Copenhagen](https://www.ku.dk/english/) under the supervision of Prof. [Serafim Bakalis](https://food.ku.dk/english/staff/?pure=en%2Fpersons%2Fserafim-bakalis(1a4bf354-3180-4450-9834-3cd052164d3c)%2Fpublications.html) and in collaboration with [Arla Foods](https://www.arla.com). From March 2024 to June 2025, I also held a Postdoctoral Research position in the Department of Food Science.

Previously, I worked (July 2021 – Feb 2024) as a postdoc in Applied Machine Learning in Plant Physiology under the supervision of [Dr. Erik Bjørnager Dam](https://di.ku.dk/english/staff/?pure=en/persons/93620), Professor, [Department of Computer Science](https://di.ku.dk/english/), University of Copenhagen, and [Dr. Kristian Thorup-Kristensen](https://plen.ku.dk/english/employees/?pure=en/persons/143157), Professor, [Department of Plant and Environmental Sciences](https://plen.ku.dk/english/), University of Copenhagen, Denmark.

I completed my Ph.D. in Applied Mathematics in 2019 at [University of Calcutta](https://www.caluniv.ac.in) under the supervision of [Dr. Soumen De](https://scholar.google.co.in/citations?user=ZwIi7oUAAAAJ&hl=en) and [Dr. Samiran Ghosh](https://research.caluniv.ac.in/researcher/samiran-ghosh). I received my M.Tech in Computer Applications from [Indian Institute of Technology, Delhi](https://home.iitd.ac.in) in 2008, and my M.Sc. in Mathematics from [Indian Institute of Technology, Bombay](https://www.iitb.ac.in) in 2005.

Before joining the postdoc, I worked as an Associate Professor at the [Institute of Engineering and Management](https://iem.edu.in), Kolkata, India.

I specialize in Machine Learning, Deep Learning, Physics-informed Machine Learning, and Data-driven Scientific Computing. I have been actively involved in developing machine learning methods that extract patterns from multimodal agriculture data in crop science through the [RadiMax](https://cropinnovation.dk/some-of-the-projects/radimax/) and [RadiBooster](https://plen.ku.dk/english/research/crop_sciences/cpps/radibooster/) projects. I am also working on fine-tuning large language models (LLMs) with retrieval-augmented generation (RAG) in generative AI.

---

## Project 1: RadiMax: Machine Learning for understanding plant root function

[Paper link](https://doi.org/10.1007/s11104-023-06253-7)  
[Code link](https://github.com/satyasaran/CropML.git)

<div style="text-align: justify; border: 2px solid black; padding: 10px;">
This project investigates the relationship between root distribution and resource uptake in crops using machine learning techniques. The study utilizes the RadiMax semi-field root-screening facility to phenotype winter wheat genotypes for root growth. Square root of planar root length density (Sqrt_pRLD) measurements are collected at different soil depths, and their correlation with deep soil nitrogen uptake and drought resilience potential is explored using machine learning models. The results demonstrate the importance of deep rooting for water and nitrogen uptake in crops.
</div>

### Results

<div id="imageContainer" style="border: 8px solid goldenrod; padding: 10px;">
    <img src="{{ '/assets/img/Fig2.jpeg' | relative_url }}" alt="Result 1" style="width: 400px;">
</div>

<button onclick="stopSlideshow()">Stop slide show</button>
<button onclick="resumeSlideshow()">Resume</button>

<script>
let currentImageIndex = 0;
const images = [
    "{{ '/assets/img/Fig2.jpeg' | relative_url }}",
    "{{ '/assets/img/Fig5a.jpeg' | relative_url }}",
    "{{ '/assets/img/Fig3a.jpeg' | relative_url }}",
    "{{ '/assets/img/Fig6a_left.jpeg' | relative_url }}"
];
const imageContainer = document.getElementById('imageContainer');
let slideshowIntervalId;

function nextImage() {
    currentImageIndex = (currentImageIndex + 1) % images.length;
    imageContainer.innerHTML = `<img src="${images[currentImageIndex]}" alt="Result ${currentImageIndex + 1}" style="width: 400px;">`;
}

function startSlideshow() {
    slideshowIntervalId = setInterval(nextImage, 3000);
}

function stopSlideshow() {
    clearInterval(slideshowIntervalId);
}

function resumeSlideshow() {
    startSlideshow();
}

startSlideshow();
</script>

---

## Project 2: RadiMax: Deep Learning for sub-soil Image analysis to investigate deep root function

In this project, our objective was to employ deep learning techniques to analyze sub-soil images and investigate the function of deep roots in plant physiology. Specifically, we utilized transfer learning with the ResNet50 architecture to develop regression and classification models for root length estimation and root function investigation.

### Results

<div class="project-images" style="border: 4px solid goldenrod; padding: 10px;">
    <img src="{{ '/assets/img/grad1.png' | relative_url }}" alt="Result 1" style="width: 600px;">
    <img src="{{ '/assets/img/grad2.png' | relative_url }}" alt="Result 2" style="width: 600px;">
    <img src="{{ '/assets/img/grad3.png' | relative_url }}" alt="Result 3" style="width: 600px;">
</div>

---

## Project 3: Solving Non-linear PDEs in Blood Flow Modelling using Physics-informed Neural Networks

[Paper link](https://doi.org/10.1016/j.matcom.2023.10.011)  
[Code Link](https://github.com/satyasaran/BurgerEvoPINN.git)

This work introduces a Python implementation for solving non-linear PDEs arising in arterial blood flow using DeepXDE. The approach analyzes perturbations in arterial blood flow, with a focus on pressure and radius variations. A mathematical model simulates viscoelastic arterial flow, incorporating long wavelength and large Reynolds number assumptions. Physics-informed deep neural networks, trained via automatic differentiation, efficiently solve these equations. Bayesian Hyperparameter Optimization identifies the optimal neural network architecture, providing an efficient and accurate alternative to numerical methods.

<div class="project-images" style="border: 4px solid goldenrod; padding: 10px;">
    <img src="{{ '/assets/img/eqn.jpeg' | relative_url }}" alt="Equation" style="width: 800px;">
</div>

### Results

<div id="imageContainer3" class="project-images" style="border: 4px solid goldenrod; padding: 10px;">
    <img src="{{ '/assets/img/pinn.jpg' | relative_url }}" alt="Result 1" style="width: 500px;">
    <img src="{{ '/assets/img/loss.jpg' | relative_url }}" alt="Result 2" style="width: 500px; display: none;">
    <img src="{{ '/assets/img/sol1.jpg' | relative_url }}" alt="Result 3" style="width: 500px; display: none;">
    <img src="{{ '/assets/img/bay.jpg' | relative_url }}" alt="Result 4" style="width: 500px; display: none;">
    <img src="{{ '/assets/img/sol2.jpg' | relative_url }}" alt="Result 5" style="width: 500px; display: none;">
    <img src="{{ '/assets/img/sol3.jpg' | relative_url }}" alt="Result 6" style="width: 500px; display: none;">
</div>

<button onclick="stopSlideshow3()">Stop slide show</button>
<button onclick="resumeSlideshow3()">Resume</button>

<script>
let currentImageIndex3 = 0;
const images3 = [
    "{{ '/assets/img/pinn.jpg' | relative_url }}",
    "{{ '/assets/img/loss.jpg' | relative_url }}",
    "{{ '/assets/img/sol1.jpg' | relative_url }}",
    "{{ '/assets/img/bay.jpg' | relative_url }}",
    "{{ '/assets/img/sol2.jpg' | relative_url }}",
    "{{ '/assets/img/sol3.jpg' | relative_url }}"
];
const imgElements3 = document.getElementById('imageContainer3').getElementsByTagName('img');
let slideshowIntervalId3;

function nextImage3() {
    imgElements3[currentImageIndex3].style.display = 'none';
    currentImageIndex3 = (currentImageIndex3 + 1) % images3.length;
    imgElements3[currentImageIndex3].style.display = 'block';
}

function startSlideshow3() {
    slideshowIntervalId3 = setInterval(nextImage3, 3000);
}

function stopSlideshow3() {
    clearInterval(slideshowIntervalId3);
}

function resumeSlideshow3() {
    startSlideshow3();
}

startSlideshow3();
</script>

---

## Project 4: Fully Automated Tumor Segmentation for Brain MRI using Multi-planar U-Net

[Paper link](https://doi.org/10.48550/arXiv.2401.06499)

Automated segmentation of distinct tumor regions is critical for accurate diagnosis and treatment planning in pediatric brain tumors. This study evaluates the efficacy of the Multi-Planner U-Net (MPUnet) approach in segmenting different tumor subregions across three challenging datasets: PED, MET, and SSA. Multi-planar information enhances segmentation accuracy. Our results show high accuracy for the tumor core class, with variability in edema and enhancing tumor regions. Further refinement and inclusion of more MRI data can improve outcomes.

<div class="project-images" style="border: 4px solid goldenrod; padding: 10px;">
    <img src="{{ '/assets/img/brain.png' | relative_url }}" alt="Brain Tumor Result" style="width: 800px;">
</div>
