# DiverseAR Datasets
This repository accompanies the workshop paper "_Advancing the Understanding and Evaluation of AR-Generated Scenes: When Vision-Language Models Shine and Stumble_", submitted to GenAI-XR 2025. It introduces **DiverseAR**, a dataset of 318 images collected from two commercial AR platforms (Amazon and Scaniverse), three AR applications (HoloLens) previously developed by our lab, and two AR applications (Apple Vision Pro and Android) specifically created for this project. 

# Dataset
The full DiverseAR dataset can be downloaded here: [https://duke.box.com/s/axx8v30a16goy7kozway1mhv1up9jcox](https://duke.box.com/s/axx8v30a16goy7kozway1mhv1up9jcox) The dataset follows the hierarchical file structure shown below:
```
images
└───android
│   │
│   └───Screenhot_202412xx-xxxxxx.png
│   ...
└───scaniverse
│   │
│   └───IMG_xxxx.PNG
│   ...
└───lab
│   │
│   └───image (x).png
│   ...
└───avp
│   │
│   └───IMG_xxxx.PNG
│   ...
└───amazon
│   │
│   └───IMG_xxxx.PNG
│   ...
└───website
│   │
│   └───Screenhot 2024-12-xx at xx.xx.xx.png
│   ...
```

_Creation:_ To evaluate the AR scene understanding capabilities of VLMs, we curated the DiverseAR dataset, specifically designed to capture a broad spectrum of AR scenarios. The dataset consists of **298 AR images** collected from diverse sources and environments. It includes 23 images captured using a custom-developed Apple Vision Pro AR application in laboratory and kitchen environments, and 151 images collected from a custom-developed Android AR application in bedroom and dining room environments. Additionally, 42 images were created in-house to explore AR-specific research topics, such as attention patterns, task-detrimental virtual content arrangements, and AR applications in surgical guidance. The dataset also features 7 images of glass objects obtained from the Amazon app's AR View, and 46 images collected from the Scaniverse app's AR View, captured in laboratory, kitchen, and dining room environments. Finally, 29 images were sourced from a website showcasing AR advertisement videos. Additionally, we included **20 non-AR images** to supplement the dataset. This comprehensive collection ensures the DiverseAR dataset supports robust analysis of AR scene understanding. 

_Details:_ The DiverseAR dataset encompasses a wide spectrum of AR and non-AR scenarios, showcasing diverse characteristics of both virtual and real-world content. Table below summarizes the key characteristics represented in the dataset, while Figure below illustrates representative examples of these characteristics. The dataset includes single or multiple instances of identical and varied real and virtual objects across various AR images. These objects span numerous classes, including **toys, food, shoes, plants, laptops, containers, and more**.

<p align="center"><img width="1000" alt="Key characteristics of the virtual and real objects in the DiverseAR dataset." src="https://github.com/BiGuideCollection/DiverseAR-Dataset/blob/main/readme_image/DiverseARtable.png"></p>

<p align="center"><img width="407" alt="Examples of key characteristics of the virtual and real objects in the DiverseAR dataset." src="https://github.com/BiGuideCollection/DiverseAR-Dataset/blob/main/readme_image/DiverseAR.png"></p>
<p align="center">Figure 1. Examples of key characteristics of the virtual and real objects in the DiverseAR dataset.</p> 


The three AR scene difficulty levels are labeled in the labeled_images.csv file.

# Acknowledgements 

The authors of this repository are Lin Duan, Yanming Xiu and Maria Gorlatova. Contact information of the authors:

* Lin Duan (lin.duan AT duke.edu)
* Yanming Xiu (yanming.xiu AT duke.edu)
* Maria Gorlatova (maria.gorlatova AT duke.edu)

This work was supported in part by NSF grants CSR-2312760, CNS-2112562 and IIS-2231975, NSF CAREER Award IIS-2046072, NSF NAIAD Award 2332744, a CISCO Research Award, a Meta Research Award, and Defense Advanced Research Projects Agency Young Faculty Award HR0011-24-1-0001. This paper has been approved for public release; distribution is unlimited. The contents of the paper do not necessarily reflect the position or the policy of the Defense Advanced Research Projects Agency. No official endorsement should be inferred.
 
