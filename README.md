# SyntheticIllusions: Pix2Pix and cycleGAN

For this project a neural network was trained on a synthetic dataset rendered using 3D game engine software (Unity Technologies, n.d.; Rodriguez, 2019). Neural networks require a large amount of high-quality labelled data. Without the infrastructure and the data collection methods of large technology companies it can be difficult to source a large enough dataset to train a neural network effectively. Therefore, synthetic datasets are a powerful tool to disrupt this disadvantage. Training using a synthetic data set allows for endless possibilities and the ability to selectively refine the final creative output. My inspiration was to create optical art such as below.

![GitHub Logo](/images/OpArt.png)

(Vaserely, 1957; Chan, 2012)

To achieve these outputs and apply optical art patterns to a variety of input images would require a technique in machine learning called image-to-image translation. Pix2pix was utilised as the implementation of image-to-image translation using a conditional adversarial network called CycleGAN (cGAN). Pix2Pix works by training the neural network on a set of related input-output image pairs to generate the target output from the input (Isola et al., 2016).  The aim was to train a neural network on image pairs of patterned 3D objects rendered using a game engine (target output) and a depth map of the rendered image as the translation layer (or input). 

![GitHub Logo](/images/ImageGeneration.gif)

A depth map is a grayscale image that contains information about the distance between the surface of objects from a given perspective. It is hoped that the network will be able to take input depth maps of any image or model and output an image with the pattern applied to create the optical effect above. 

Training Pairs

![GitHub Logo](/images/depthpairs.gif)

Outputs

![GitHub Logo](/images/head.gif) ![GitHub Logo](/images/hand.gif)

References:

Chan, L. (2012). Hand Op Art. Retrieved from https://www.deviantart.com/x-luna-chan-x/art/Hand-Op-Art-305612272.

Isola, P., Zhu, J. Y., Zhou, T., & Efros, A. A. (2016). Image-to-image translation with conditional adversarial networks. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 1125-1134).

Unity Technologies. (n.d.). Image Synthesis for Machine Learning. Retrieved from https://bitbucket.org/Unity-Technologies/ml-imagesynthesis/src.

Vaserely, V. (1957). VEGA III [Painting, Kinetic art, Oil on canvas]. Guggenheim, New York, NY.
