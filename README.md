# STM-feature-classificaton-ANN
Neural network for feature classification in STM images

The desired result is to use an FCN (fully convolutional network) to segment STM images using a small dataset (~10^1 imgs) with varying feature size scales. The goal is to create a prototype program that classifies molecular features in STM (scanning tunneling microscopy) images to demonstrate the potential of computer vision networks to accelerate research through reducing time spent manually labeling images.

Results:
- MLP (multilayer perceptron/"vanilla NN") used to segment synthetic STM-like single-feature images
- FCN performing accurate segmentations on small dataset with noise and feature scale variations, all of which are typical of experiments

STM and more broadly, SPM (scanning probe microscopy), are tools used to probe molecular properties on nanometer scales. A bias voltage is imposed between a probe tip and a conductive surface containing sample, and current is tunneled that reflects sample local density of electron states (LDOS). Typical ambient temperature STM image datasets often have high noise due to probe drift, sample contamination, variable LDOS corresponding to a same species, however for simplicity in establishing a first result, I chose a relatively high-quality set of images. 

A high-quality STM image of two organic molecules self-assembling on graphite:


<img src="typicalSTM.jpg" width=300>
