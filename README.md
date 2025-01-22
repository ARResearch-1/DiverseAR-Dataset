# DiverseAR Datasets
This repository accompanies the workshop paper "_Advancing the Understanding and Evaluation of AR-Generated Scenes: When Vision-Language Models Shine and Stumble_", accepted by GenAI-XR 2025. It introduces **DiverseAR**, a dataset of 318 images collected from two commercial AR platforms (Amazon and Scaniverse), three AR applications (HoloLens, Magic Leap, Android) previously developed by our lab, and two AR applications (Apple Vision Pro and Android) specifically created for this project. 

# Dataset
The full DiverseAR dataset can be downloaded here: [https://duke.box.com/s/kdh4ns4ep2a3sjde05prk0hik0juzz9f](https://duke.box.com/s/kdh4ns4ep2a3sjde05prk0hik0juzz9f). The dataset follows the hierarchical file structure shown below:
```
DiverseAR_dataset
└───images
│   │
│   └───image_1.png
│   └───image_2.png
│   ...
└───DiverseAR_annotation.csv
```

DiverseAR_annotation.csv contains the columns ["image_name", "AR/NonAR", "source", "complexity_level"], which represent the image name, whether the image is an AR or Non-AR image, the source platform, and the complexity level, respectively. A portion of the unaugmented raw data is available for download here: [https://duke.box.com/s/915pors2tn4dtrazfjesd2k7vm73b8eg](https://duke.box.com/s/915pors2tn4dtrazfjesd2k7vm73b8eg)

_Creation:_ To evaluate the AR scene understanding capabilities of VLMs, we curated the DiverseAR dataset, specifically designed to capture a broad spectrum of AR scenarios. The dataset consists of **298 AR images** collected from diverse sources and environments. It includes 23 images captured using a custom-developed Apple Vision Pro AR application in laboratory and kitchen environments, and 151 images collected from a custom-developed Android AR application in bedroom and dining room environments. Additionally, 42 images were created in-house to explore AR-specific research topics, such as attention patterns, task-detrimental virtual content arrangements, and AR applications in surgical guidance. The dataset also features 7 images of glass objects obtained from the Amazon app's AR View, and 46 images collected from the Scaniverse app's AR View, captured in laboratory, kitchen, and dining room environments. Finally, 29 images were sourced from a website showcasing AR advertisement videos. Additionally, we included **20 non-AR images** to supplement the dataset. This comprehensive collection ensures the DiverseAR dataset supports robust analysis of AR scene understanding. 

_Details:_ The DiverseAR dataset encompasses a wide spectrum of AR and non-AR scenarios, showcasing diverse characteristics of both virtual and real-world content. Table below summarizes the key characteristics represented in the dataset, while Figure below illustrates representative examples of these characteristics. The dataset includes single or multiple instances of identical and varied real and virtual objects across various AR images. These objects span numerous classes, including **toys, food, shoes, plants, laptops, containers, and more**.

<p align="center"><img width="1000" alt="Key characteristics of the virtual and real objects in the DiverseAR dataset." src="https://github.com/BiGuideCollection/DiverseAR-Dataset/blob/main/readme_image/DiverseARtable.png"></p>

<p align="center"><img width="407" alt="Examples of key characteristics of the virtual and real objects in the DiverseAR dataset." src="https://github.com/BiGuideCollection/DiverseAR-Dataset/blob/main/readme_image/DiverseAR.png"></p>
<p align="center">Figure 1. Examples of key characteristics of the virtual and real objects in the DiverseAR dataset.</p> 

# Citation

If you use DiverseAR dataset in an academic work, please cite: 

```
@inproceedings{DiverseAR,
  title={Advancing the Understanding and Evaluation of AR-Generated Scenes: When Vision-Language Models Shine and Stumble},
  author={Duan, Lin, and Xiu, Yanming and Gorlatova, Maria},
  booktitle={Proceedings of IEEE VR GenAI-XR 2025},
  year={2025}
 }
 ```

# Acknowledgements 

The authors of this repository are Lin Duan, Yanming Xiu and Maria Gorlatova. Contact information of the authors:

* Lin Duan (lin.duan AT duke.edu)
* Yanming Xiu (yanming.xiu AT duke.edu)
* Maria Gorlatova (maria.gorlatova AT duke.edu)

We thank our user study participants for their invaluable assistance in this research. This work was supported in part by NSF grants CSR-2312760, CNS-2112562 and IIS-2231975, NSF CAREER Award IIS-2046072, NSF NAIAD Award 2332744, a CISCO Research Award, a Meta Research Award, Defense Advanced Research Projects Agency Young Faculty Award HR0011-24-1-0001, and the Army Research Laboratory under Cooperative Agreement Number W911NF-23-2-0224. The views and conclusions contained in this document are those of the authors and should not be interpreted as representing the official policies, either expressed or implied, of the Defense Advanced Research Projects Agency, the Army Research Laboratory, or the U.S. Government. This paper has been approved for public release; distribution is unlimited. No official endorsement should be inferred. The U.S. Government is authorized to reproduce and distribute reprints for Government purposes notwithstanding any copyright notation herein.
 
