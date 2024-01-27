---
layout: about
title: about
permalink: /
subtitle: 

profile:
  align: right
  image: satyaku.jpeg
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

I have been collaborating with my PhD supervisor [Dr. Soumen De](https://scholar.google.co.in/citations?user=ZwIi7oUAAAAJ&hl=en), Department of Applied Mathematics, University of Calcutta and have supervised [Bivas Bhaumik](https://scholar.google.com/citations?user=FfG_kKQAAAAJ&hl=en&authuser=3) (Currently Assistant Prifessor at Department of Mathematics, [NIT Rourkela](https://nitrkl.ac.in),  during his PhD. Currently I am supervising [Susmita Saha](https://www.researchgate.net/profile/Susmita-Saha-16) and Soumini Dolui for their PhD at University of Calcutta, India.
For more details:
[Download CV](assets/pdf/CV_satyasaran.pdf)


<br>

<div style="background-color: #baffea; padding: 10px; border: 1px solid #ddd;">
    <h2 style="margin: 0;font-weight: bold;">Current Research Projects </h2>
</div>
<br>
## Project 1: RadiMax: Machine Learning for understanding plant root function
<br>
[Paper link:](https://doi.org/10.1007/s11104-023-06253-7) 
<br>
[code link](https://github.com/satyasaran/CropML.git)

This project investigates the relationship between root distribution and resource uptake in crops using machine learning techniques. The study utilizes the RadiMax semi-field root-screening facility to phenotype winter wheat genotypes for root growth. Square root of planar root length [CNN, Deep learning was used to extract the root length from sub-soil images] density (Sqrt_pRLD) measurements are collected at different soil depths, and their correlation with deep soil nitrogen uptake and drought resilience potential is explored using machine learning models. The results demonstrate the importance of deep rooting for water and nitrogen uptake in crops.
### Results
<div id="imageContainer" style="border: 8px solid goldenrod; padding: 10px;">
    <img src="/assets/img/Fig2.jpeg" alt="Result 1" style="width: 400px;">
</div>

<button onclick="stopSlideshow()">Stop slide show</button>
<button onclick="resumeSlideshow()">Resume</button>

<script>
    let currentImageIndex = 0;
    const images = [
        "/assets/img/Fig2.jpeg",
        "/assets/img/Fig5a.jpeg",
        "/assets/img/Fig3a.jpeg",
        "/assets/img/Fig6a_left.jpeg"
    ];
    const imageContainer = document.getElementById('imageContainer');
    let slideshowIntervalId;

    function nextImage() {
        currentImageIndex = (currentImageIndex + 1) % images.length;
        const currentImage = images[currentImageIndex];
        imageContainer.innerHTML = `<img src="${currentImage}" alt="Result ${currentImageIndex + 1}" style="width: 400px;">`;
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


<br>
## Project 2: RadiMax: Deep Learning for sub-soil Image analysis to investigate deep root function 
<br>

In this project, our objective was to employ deep learning techniques to analyze sub-soil images and investigate the function of deep roots in plant physiology. Specifically, we utilized transfer learning with the ResNet50 architecture to develop regression and classification models for root length estimation and root function investigation.


### Results

Here are some images showcasing the results:

<div class="project-images" style="border: 4px solid goldenrod; padding: 10px;">
    <img src="/assets/img/grad1.png" alt="Result 1" style="width: 600px;">
    <img src="/assets/img/grad2.png" alt="Result 2" style="width: 600px;">
    <img src="/assets/img/grad3.png" alt="Result 3" style="width: 600px;">
</div>
---

<br>
## Project 3: Solving Non-linear partial differential equations in Blood flow modelling using Physics-informed Neural network
<br>
[Paper link](https://doi.org/10.1016/j.matcom.2023.10.011) 
<br>
[Code Link](https://github.com/satyasaran/BurgerEvoPINN.git)

This work introduces a Python implementation of solution of non-liner PDEs arising in the process of arterial blood flow using DeepXDE. The proposed deep learning approach analyzes perturbations in arterial blood flow, with a focus on pressure and radius variations. The research develops a mathematical model for simulating viscoelastic arterial flow, incorporating long wavelength and large Reynolds number assumptions. Leveraging the reductive perturbation method, the study derives nonlinear evolutionary equations for medium resistance, elastic properties, and wall viscosity. By employing state-of-the-art physics-informed deep neural networks, trained via automatic differentiation, the implementation efficiently solves these equations. Bayesian Hyperparameter Optimization identifies the optimal neural network architecture, providing an efficient and accurate alternative to numerical methods for medical machine learning applications.
### Results

Here are some images showcasing the results: [Image sources: published Paper link](https://doi.org/10.1016/j.matcom.2023.10.011)
<div id="imageContainer3" class="project-images" style="border: 4px solid goldenrod; padding: 10px;">
    <img src="/assets/img/pinn.jpg" alt="Result 1" style="width: 500px;">
    <img src="/assets/img/loss.jpg" alt="Result 2" style="width: 500px; display: none;">
    <img src="/assets/img/sol1.jpg" alt="Result 3" style="width: 500px; display: none;">
    <img src="/assets/img/bay.jpg" alt="Result 4" style="width: 500px; display: none;">
    <img src="/assets/img/sol2.jpg" alt="Result 5" style="width: 500px; display: none;">
    <img src="/assets/img/sol3.jpg" alt="Result 6" style="width: 500px; display: none;">
</div>

<button onclick="stopSlideshow3()">Stop slide show</button>
<button onclick="resumeSlideshow3()">Resume</button>

<script>
    let currentImageIndex3 = 0;
    const images3 = [
        "/assets/img/pinn.jpg",
        "/assets/img/loss.jpg",
        "/assets/img/sol1.jpg",
        "/assets/img/bay.jpg",
        "/assets/img/sol2.jpg",
        "/assets/img/sol3.jpg"
    ];
    const imageContainer3 = document.getElementById('imageContainer3');
    const imgElements3 = imageContainer3.getElementsByTagName('img');
    let slideshowIntervalId3;

    // Function to display the next image for Project 3
    function nextImage3() {
        // Hide the current image
        imgElements3[currentImageIndex3].style.display = 'none';
        // Move to the next image index
        currentImageIndex3 = (currentImageIndex3 + 1) % images3.length;
        // Show the next image
        imgElements3[currentImageIndex3].style.display = 'block';
    }

    // Start the slideshow for Project 3
    function startSlideshow3() {
        slideshowIntervalId3 = setInterval(nextImage3, 3000);
    }

    // Stop the slideshow for Project 3
    function stopSlideshow3() {
        clearInterval(slideshowIntervalId3);
    }

    // Resume the slideshow for Project 3
    function resumeSlideshow3() {
        startSlideshow3();
    }

    // Start the slideshow for Project 3 initially
    startSlideshow3();
</script>



<br>
## Project 4: Fully Automated Tumor Segmentation for Brain MRI data using Multiplanner UNet
<br>
[Paper link](https://doi.org/10.48550/arXiv.2401.06499)

<br>
<div class="project-images" style="border: 4px solid goldenrod; padding: 10px;">
    <img src="/assets/img/brain.png" alt="Result 1" style="width: 800px;">
</div>

Automated segmentation of distinct tumor regions is critical for accurate diagnosis and treatment planning in pediatric brain tumors. This study evaluates the efficacy of the Multi-Planner U-Net (MPUnet) approach in segmenting different tumor subregions across three challenging datasets: Pediatrics Tumor Challenge (PED), Brain Metastasis Challenge (MET), and Sub-Sahara-Africa Adult Glioma (SSA). These datasets represent diverse scenarios and anatomical variations, making them suitable for assessing the robustness and generalization capabilities of the MPUnet model. By utilizing multi-planar information, the MPUnet architecture aims to enhance segmentation accuracy. Our results show varying performance levels across the evaluated challenges, with the tumor core (TC) class demonstrating relatively higher segmentation accuracy. However, variability is observed in the segmentation of other classes, such as the edema and enhancing tumor (ET) regions. These findings emphasize the complexity of brain tumor segmentation and highlight the potential for further refinement of the MPUnet approach and inclusion of MRI more data and preprocessing.
