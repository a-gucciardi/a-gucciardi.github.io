---
title: Siamese Networks in medical imagery CNN-based comparative study for brain symmetry scoring
description: A Gucciardi, S El Ghazouali, V Groznik, U Michelucci. 
date: 2025-01-24 
image: brain.png
categories:
    - Article
links:
  - title: Paper 
    description: 
    website: https://drive.google.com/file/d/1256e58XD3KemZFU0wO0askTHJwqUKaSp/view?usp=drive_link
    image: https://arxiv.org/static/browse/0.3.4/images/icons/smileybones-pixel.png
---
**PhD Thesis paper.**  
**Responsible for the Data annotation/preparation - Code (PyTorch) - Writing - Figures**
<H1>Automated Neonatal MRI Symmetry Analysis with Siamese CNNs</H1>

Early detection of developmental abnormalities in the neonatal brain is crucial for timely diagnosis and intervention. However, analyzing symmetry in neonatal brain MRIs remains a challenging task due to the unique imaging characteristics of newborns—such as smaller brain size, rapid developmental changes, and lower tissue contrast. While deep learning has revolutionized medical imaging, existing models often struggle to effectively handle these specific challenges in neonatal scans.

In this research, we systematically evaluate the performance of Siamese neural networks for automated symmetry analysis in neonatal brain MRIs. Siamese networks are particularly well-suited for tasks involving pairwise comparisons, making them ideal for detecting subtle hemispheric asymmetries.

<H2>Benchmarking State-of-the-Art Architectures</H2>
We compared five prominent deep learning backbone architectures integrated into the Siamese network framework:
* ResNet
* ResNeXt
* MobileNet
* EfficientNet
* VGG

<H3>Labelling & simulations</H3>
To rigorously evaluate these models, we curated a novel dataset comprising 3,150 annotated axial brain views of neonates. We then introduced controlled asymmetry simulations into the images, ranging in size from 1 mm² to 20 mm², enabling us to benchmark detection capabilities at varying levels of difficulty.
 
<H3>Training Protocol: Progressive Asymmetry Simulation</H3>
A key innovation in our study is a progressive training protocol. Rather than exposing the models to large asymmetries from the start, we gradually increase the simulated asymmetry during training. This approach mirrors a curriculum learning strategy, helping the networks adapt more effectively and improving their ability to detect subtle abnormalities.

<H3>Key Findings</H3>
Our experiments yielded several important insights:

* VGG-based Siamese architectures outperformed all other models across most asymmetry levels.

* Detection accuracy increased with asymmetry size, reaching:

    * 76% accuracy for 7 mm² asymmetries

    *  99% accuracy for asymmetries larger than 13.5 mm²

Interestingly, models trained on medium-range asymmetries (e.g., 7–13 mm²) showed better generalization to both smaller and larger asymmetries, highlighting the importance of balanced training data.

<H3>Contributions to Neonatal Neuroimaging</H3>
This research offers both practical and theoretical contributions to the field:

* A publicly available, annotated dataset for neonatal symmetry analysis
* A comparative benchmark of deep learning architectures tailored to neonatal imaging
* A training methodology that enhances detection performance through progressive learning

By addressing a critical gap in neonatal MRI analysis, our work supports the development of more sensitive, robust, and clinically viable diagnostic tools. With continued refinement, automated symmetry analysis could play a vital role in early detection of neurodevelopmental disorders, ultimately improving outcomes for at-risk infants.