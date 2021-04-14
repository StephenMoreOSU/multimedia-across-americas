# Comparing Modern Video Compression Techniques

## Introduction

Compression, in all of its forms, allows for more efficient delivery of digital information. There are two main types of compression: Lossless compression, and Lossy compression. As of all things, each situation requires a different type of compression, and within each type, there are multiple ways to approach the task. Modern compression techniques, such as HEVC (High-efficiency video coding, also known as H.265) are lossy compression techniques. This survey will analyze and evaluate the multiple available modern standards of video compression, and disclose the tradeoffs and limitations of each of the formats studied.

## Motivation

Compression is needed to support the many multimedia applications used by engineers across diverse fields in ECE. Understanding the tradeoffs between cutting-edge compression techniques is important if one intends to implement new designs under the tight engineering constraints of the industry.

## Background

Deep Neural Networks (DNNs) have become extremely popular for solving diverse sets of challenges including natural language processing, image recognition, autonomous vehicles, and classification problems which are harder for non-data-driven algorithms to solve. The availability of the datasets needed to train such networks has also increased dramatically in recent years. The usefulness creates a demand for such DNNs to be used across diverse environments with vastly different hardware and bandwidth requirements. Strict hardware requirements such as the amount of memory available are a huge constraint when attempting to apply DNN applications to embedded systems. A classical example of an object detection DNN is AlexNet which requires 240MB of space. While 240MB may be available on higher-end embedded systems, there is still more that is needed. What if multiple networks need to be used simultaneously? (often the case in autonomous vehicles), what if one wants to deploy DNN applications across many lower-cost embedded devices with less memory? What if such embedded devices are communicating with servers over the internet to execute their applications? There will always be a demand for more computers, and the memory required to use DNN applications either over the cloud or on the edge is still a bottleneck for certain applications. This is why it is important to look at the cutting edge of DNN compression and compare the engineering tradeoffs between methodologies.

The old mainstream method of video compression, H.264, was developed in 2003. The newer compression method, H.265, uses 64x64 macroblocks while H.264 uses 16x16 macroblocks. The larger macroblocks allow for better compression efficiency at all resolutions, especially the higher resolutions that most consumers are using today, H.265 supports up to 8k (8192 pixels x 4320 pixels) video compression. H.265 also has better motion prediction and compensation. H.265 uses 33 directions of motion for motion/frame prediction, while H.264 only uses nine directions of motion. H.265 supports parallel processing. Intel has produced processors with instruction sets for encoding and decoding H.265 video, showing a promising future for H.265 even though H.264 is still more commonly used.

AV1 is nearly twice as efficient as H.264, works with high-quality video, has no licensing fee, works with bandwidth constraints. H.265 has uncertainties around its licensing fees making it untenable for an average consumer. AV1’s goal is to replace H.264 and compete with H.265 so the high-quality video can be shared freely and efficiently on the internet. Companies and creators have to pay a royalty to compress and decompress with H.264 and H.265.

## Taxonomy

For each category of compression:
1. Take 3 examples, find fundamental data from research papers, or if needed clone the repo and get benchmarks ourselves
1. With gathered data, create visualizations that can compare the findings in an understandable way
1. Compare the examples using the tradeoff criteria 
1. Make a conclusion about which compression methodology is good to use in which situation
1. Compare new techniques with a baseline that is as standard as possible (H.264 for video) 

Tradeoffs for comparison:
* Usability - How easy is it to use? How widespread is the support for the compression?
* Compression density - How much does it reduce file size?
* Compression Computational efficiency - How computationally demanding is the process? How long does it take to compress?
* Support moving forward - How maintained is the methodology?
* Lossy vs Lossless

## Task Commissioning

* Everyone
  * Research
  * Midterm Report
  * Final Report 


## References

[<sub>InterDigitalInc, “InterDigitalInc/CompressAI,” GitHub. [Online]. Available: https://github.com/InterDigitalInc/CompressAI  [Accessed: 13-Apr-2021].</sub>](https://github.com/InterDigitalInc/CompressAI)

[<sub>C. Shorten, “Deep Compression,” Medium, 10-Jun-2019. [Online]. Available: https://towardsdatascience.com/deep-compression-7b771b3aa773  [Accessed: 13-Apr-2021].</sub>](https://towardsdatascience.com/deep-compression-7b771b3aa773)

[<sub>Y. Cheng, D. Wang, P. Zhou, and T. Zhang, “A Survey of Model Compression and Acceleration for Deep Neural Networks,” arXiv.org, 14-Jun-2020. [Online]. Available: https://arxiv.org/abs/1710.09282v9  [Accessed: 13-Apr-2021].</sub>](https://arxiv.org/abs/1710.09282v9)

[<sub>S. Han, H. Mao, and W. J. Dally, “Deep Compression: Compressing Deep Neural Networks with Pruning, Trained Quantization and Huffman Coding,” arXiv.org, 15-Feb-2016. [Online]. Available: https://arxiv.org/abs/1510.00149  [Accessed: 13-Apr-2021].</sub>](https://arxiv.org/abs/1510.00149)

[<sub>A.  Fox, “What is H.265, and Why Is It Better than H.264?,” Make Tech Easier, 07-Aug-2017. [Online]. Available: https://www.maketecheasier.com/h265-vs-h264/#:~:text=increased%20macroblock%20size.-,H.,encoding%20efficiency%20at%20all%20resolutions  [Accessed: 13-Apr-2021].</sub>](https://www.maketecheasier.com/h265-vs-h264/#:~:text=increased%20macroblock%20size.-,H.,encoding%20efficiency%20at%20all%20resolutions)

[<sub>“AV1 is a royalty-free video compression format for the web,” Mozilla Research. [Online]. Available: https://research.mozilla.org/av1-media-codecs/  [Accessed: 13-Apr-2021].</sub>](https://research.mozilla.org/av1-media-codecs/)

## The Team

Stephen More (Leader) - [mores@oregonstate.edu](mailto:mores@oregonstate.edu)   

<img src="https://media.discordapp.net/attachments/829757911298342925/831967460247994368/StephenMore_-_cropped.jpg" data-canonical-src="https://media.discordapp.net/attachments/829757911298342925/831967460247994368/StephenMore_-_cropped.jpg" width="250" height="250" />

Felipe Orrico Scognamiglio - [orricosf@oregonstate.edu](mailto:orricosf@oregonstate.edu)   

<img src="https://cdn.discordapp.com/attachments/829757911298342925/831967603378880522/Felipe_Beaver.png" data-canonical-src="https://cdn.discordapp.com/attachments/829757911298342925/831967603378880522/Felipe_Beaver.png" width="250" height="250" />

Jacob Gillette - [gilletja@oregonstate.edu](mailto:gilletja@oregonstate.edu)   

<img src="https://media.discordapp.net/attachments/829757911298342925/831968062625415288/JacobG_-_cropped.jpg" data-canonical-src="https://media.discordapp.net/attachments/829757911298342925/831968062625415288/JacobG_-_cropped.jpg" width="250" height="250" />


Emilio Magaña - [maganem@oregonstate.edu](mailto:maganem@oregonstate.edu) 

<img src="https://media.discordapp.net/attachments/829757911298342925/831970096230432848/emilio_-_cropped.jpg" data-canonical-src="https://media.discordapp.net/attachments/829757911298342925/831970096230432848/emilio_-_cropped.jpg" width="250" height="250" />

Hassan Alabdulaziz - [alabduha@oregonstate.edu](mailto:alabduha@oregonstate.edu)  

<img src="https://media.discordapp.net/attachments/829757911298342925/831972317629382666/Hassan_-_cropped.jpg" data-canonical-src="https://media.discordapp.net/attachments/829757911298342925/831972317629382666/Hassan_-_cropped.jpg" width="250" height="250" />


## Contact

Stephen More (Leader) - [mores@oregonstate.edu](mailto:mores@oregonstate.edu)  
Emilio Magaña - [maganem@oregonstate.edu](mailto:maganem@oregonstate.edu)  
Jacob Gillette - [gilletja@oregonstate.edu](mailto:gilletja@oregonstate.edu)  
Felipe Orrico Scognamiglio - [orricosf@oregonstate.edu](mailto:orricosf@oregonstate.edu)  
Hassan Alabdulaziz - [alabduha@oregonstate.edu](mailto:alabduha@oregonstate.edu)  

