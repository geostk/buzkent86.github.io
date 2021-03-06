---
title: ""
permalink: /news/
author_profile: true
redirect_from:
  - /news
---

{% include base_path %}

- Our paper on high-speed scale-adaptive object tracking (>300fps) has been accepted to the *IEEE Winter Conference on Applications of Computer Vision (WACV18) 2018*!

	- Uzkent, Burak, and Seo, YoungWoo "EnKCF : Ensemble of Kernelized Correlation Filters for Object Tracking in High Speed" [arxiv](https://arxiv.org/pdf/1801.06729.pdf)

        - [Demo Video 1](https://www.youtube.com/embed/dWeIbECiVkY?ecver=1), [Demo Video 2](https://www.youtube.com/embed/ZCnAjxJkseY?ecver=1), [Demo Video 3](https://www.youtube.com/embed/hAxA903YH2Y?ecver=1), [Demo Video 4](https://www.youtube.com/embed/h-yXx1A2dL0?ecver=1)

	![Tracking_Framework](../images/EnKCF_Framework.png)

- I am currently working on the potential applications of Kernelized Correlation Filter to hyperspectral aerial videos for object tracking. Additionally, I work on vehicle detection in the *Wide-Area-Motion-Imagery (WAMI)* platform by training a Deep Convolutional Neural Network on a *synthetic dataset* generated by the DIRSIG software. This way, one can detect vehicles in WAMI platform without using any WAMI training data. Some of the positive samples in synthetic (DIRSIG) and real dataset (WAMI) can be seen in the figure below. The trained Deep Learning model can classify the WAMI samples with `93%` accuracy.

	![positive_samples](../images/positives_vehicle_detection.jpg)

- We submitted our paper on high speed object tracking to the *Winter Application of Computer Vision Conference 2018*. Some experiments on the UAV123 dataset is attached below. The experiments are carried out on an *I5, 2.7 GHz processor* in *C++* platform on a Ubuntu OS. We propose a scale adaptive-tracker that can run on average at `416 fps` on the *UAV123 dataset*, that is faster than the vanilla form KCF tracker operating at `380 fps` in the same platform on the *UAV123 dataset*. Such tracker can then be run on a low-end platform at real-time (`30 fps`) unlike most of the state-of-the-art trackers. All the KCF driven trackers handle the scale update in a computationally demanding way, reducing the run-time performance from multiple hundreds of fps to less than a hunder fps. On the other hand, the proposed scale-adaptive tracker is as efficient as original KCF tracker, running at even slightly higher speed than the original KCF on the *UAV123 dataset*.

	- Uzkent, Burak, and Seo, YoungWoo "EnKCF : Ensemble of Kernelized Correlation Filters for Object Tracking in High Speed" [Abstract](abstract_wacv18.pdf)

- Our paper is accepted to the *Perception Beyond the Visible Spectrum Workshop in conjunction with the Computer Vision and Pattern Recognition Conference 2017*
	
	- Uzkent, Burak, Aneesh Rangnekar, Matthew J. Hoffman, and Anthony Vodacek. "Aerial Vehicle Tracking by Adaptive Fusion of Hyperspectral Likelihoods Maps"

	![Tracking_Framework](../images/CVPRW17_Tracking.png)

- Our [Hyperspectral Aerial Video Set](https://buzkent86.github.io/datasets/) for vehicle tracking is uploaded. Please cite the paper listed below if you use this dataset in your research. Our dataset also contains the ground truth files of the vehicles in the scene. You can download the C detection module coupled to MATLAB tracking module in this [link](https://github.com/buzkent86/CVPRW17_Paper_Code).

	- Uzkent, Burak, Matthew J. Hoffman, and Anthony Vodacek. "Real-Time Vehicle Tracking in Aerial Video Using Hyperspectral Features." In *Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops*, pp. 36-44. 2016.

	![Tracking_Framework](../images/CVPRW16_Tracking.png)

- I defended my Ph.D. thesis on "Aerial Vehicle Tracking using a Multi-modal Optical Sensor" as of May 16, 2016. I would like to thank my thesis committee and my advisor Dr. Hoffman and co-adviser Dr. Vodacek for their supervision throughout my Ph.D. You can download my presentation [here](../files/Thesis.Defense.pdf)

- I finished my internship at *Huawei R&D* where I worked on representing people with face-only and contextual features to classify individuals in a photo album as strangers and family members. The second part of my work included designing an album-specific classifier to assign sematic roles to family `members. My work also includes designing a general conditional random field graph based approach where several attributes about the individuals, and pairs are utilized to assign semantic roles. You can find an experiment on a family picture with strangers in the figure below. To learn contextual features, the ZFNet (Improved AlexNet) is fine-tuned on the People in Photo Album Dataset on three different areas including context. You can find the Caffe fine-tuning prototxt files in this [link](https://github.com/buzkent86/AlexNet_FineTuned_PersonRecognition). For the face-only area, the pre-trained *FaceNet* model, an end-to-end face verification model, is used.

	![obama_family](../images/Obama_Family.jpg)

- Our journal paper titled "Integrating Hyperspectral Likelihoods in a Multi-dimensional Assignment Algorithm for Aerial Vehicle Tracking" has been accepted by the *IEEE Journal of Selected Topics in Remote Sensing and Observation*. In this [link](https://www.youtube.com/watch?v=scRQjEMGSRE), you can find an example of single target tracking from a fixed aerial platform.

- For short term (2014 Summer), I worked on *3-D Cardiac segmentation using MRI slices*. I presented our paper in the IEEE Western New York Image Processing Workshop. Below, you can visualize some results on canine (left) and sheep (right) heart segmentation. C++ implementation can be found in this [link](https://github.com/buzkent86/3D_MRI_Segmentation).

	- Uzkent, Burak, Matthew J. Hoffman, Elizabeth Cherry, and Nathan Cahill. "3-D MRI cardiac segmentation using graph cuts." In *Image and Signal Processing Workshop (WNYISPW)*, 2014 IEEE Western New York, pp. 47-51. IEEE, 2014.

	Canine Heart             |  Sheep Heart
	:-------------------------:|:-------------------------:
	![canine_heart](../images/Canine_Heart_Segmentation.png)  |  ![sheep_heart](../images/Sheep_Heart_Segmentation.png)
