+ **ImageNet Classification with Deep Convolutional Neural Networks**  
  2012 - (2019/04/04: 37662) - [Alex Krizhevsky] [Ilya Sutskever] [Geoffrey E. Hinton]
  - 
  <!-- - The architecture of our network contains eight learned layers - five convolutional and three fully-connected.
  - ReLU Nonlinearity; Training on Multiple GPUs; Local Response Normalization; Overlapping Pooling
  - https://code.google.com/archive/p/cuda-convnet/ -->
+ **Caffe: Convolutional Architecture for Fast Feature Embedding**  
  2014 - (2019/04/04: 10337) - [Yangqing Jia] [Evan Shelhamer] [Jeff Donahue] [Sergey Karayev] [Jonathan Long] [Ross Girshick] [Sergio Guadarrama] [Trevor Darrell]
  - 
+ **Rich featrue hierarchies for accurate object detection and semantic segmentation**  
  2014 - (2019/04/04: 7908) - [Ross Girshick] [Jeff Donahue] [Trevor Darrell] [Jitendra Malik]
  - 
  <!-- - **R-CNN: Regions with CNN features**
  - Our approach combines two key insights: (1) one can apply high-capacity convolutional neural networks (CNNs) to bottom-up region proposals in order to localize and segment objects and (2) when labeled training data is scarce, supervised pre-training for an auxiliary task, followed by domain-specific fine-tuning, yields a significant performance boost.
  - http://www.rossgirshick.info/ -->
+ **Spatial Pyramid Polling in Deep Convolutional Networks for Visual Recognition**  
  2015 - (2019/04/04: 2518) - [Kaiming He] [Xiangyu Zhang] [Shaoqing Ren] [Jian Sun]
  - 
+ **Fast R-CNN**  
  2015 - (2019/04/04: 4950) - [Ross Girshick]
  - 
+ **Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks**  
  2015 - (2019/04/04: 8591) - [Shaoqing Ren] [Kaiming He] [Ross Girshick] [Jian Sun]
  - 
+ **You Only Look Once: Unified, Real-Time Object Detection**  
  2016 - (2019/04/04: 3712) - [Joseph Redmon] [Santosh Divvala] [Ross Girshick] [Ali Farhadi]
  - 
  <!-- - A single convolutional network simultaneously predicts multiple bounding boxes and class probabilities for those boxes. YOLO trains on full images and directly optimizes detection performance.
  - First, YOLO is extremely fast. Since we frame detection as a regression problem we don’t need a complex pipeline. We simply run our neural network on a new image at test time to predict detections.
  - Second, YOLO reasons globally about the image when making predictions. Unlike sliding window and region proposal-based techniques, YOLO sees the entire image during training and test time so it implicitly encodes contextual information about classes as well as their appearance.
  - Third, YOLO learns generalizable representations of objects. When trained on natural images and tested on artwork, YOLO outperforms top detection methods like DPM and R-CNN by a wide margin. -->
  - https://pjreddie.com/darknet/yolo/
+ **SSD: Single Shot MultiBox Detector**  
  2016 - (2019/04/03: 3346) - [Wei Liu] [Dragomir Anguelov] [Dumitru Erhan] [Christian Szegedy]
  - 
  <!-- - The core of SSD is predicting category scores and box offsets for a fixed set of default bounding boxes using small convolutional filters applied to feature maps.
  - To achieve high detection accuracy we produce predictions of different scales from feature maps of different scales, and explicitly separate predictions by aspect ratio.
  - These design features lead to simple end-to-end training and high accuracy, even on low resolution input images, further improving the speed vs accuracy trade-off.
  - https://github.com/weiliu89/caffe/tree/ssd -->
