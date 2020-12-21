# Neural-Style-Transfer-Using-VGG-19

You can visit our jupyter notebook [here](https://github.com/Junyan-Guo/Neural-Style-Transfer-Using-VGG-19/blob/main/Notebook/trials_20201220.ipynb).

### Introduction
Though the performance of neural style transfer learning is hard to quantify, we find a parameter set that generates "content-style-balanced" images using VGG-19 network with TensorFlow. We finally implement the algorithm and develop a notebook that is efficient to tune interested parameters with a GPU.

We studied on the effects of base images, layers, weight, optimizer, iterations, and total variation loss. By controlling variables, the parameter set: $\alpha /\beta$  = 1e5 (e.g., content loss weight = 1, style loss weight = 1e-5), content layer = block5-conv2, Adam optimizer with learning rate = 5, iteration =  2000 steps, and select content image as the base image, meets our standard. Apart from the default set, we find that choosing pure black and white images as base image can result in brightness difference. Also, when starting from a white noise picture, a convolutional layer in block 4 has better performance. If a smooth output image is needed, then a total variation loss with weight 1e-3 can be applied. Furthermore, we explored how the variation of these parameters will influence the final output image, therefore, we can utilize those regularities in specific neural style transfer application situations.

### Group memebers
*******************
Chang Gu (cg3168)

Junyan Guo (jg4184)

Binyao Cheng (bc2866)

Ruichen Tang (rt2756)
*******************

<img src="Sample output/Trained Images.png" alt="Structure" width="800"/>

  ### Folders

The [**Note book**](https://github.com/Junyan-Guo/Neural-Style-Transfer-Using-VGG-19/tree/main/Notebook) folder contains our notebook, which is efficient for parameter tuning.

The [**Sample output**](https://github.com/Junyan-Guo/Neural-Style-Transfer-Using-VGG-19/tree/main/Sample%20output) folder is consists of the images that are conculded in our paper.

The [**Plot VGG-19**](https://github.com/Junyan-Guo/Neural-Style-Transfer-Using-VGG-19/tree/main/Plot%20VGG-19) folder saves the code that we generated the network structure plot.
