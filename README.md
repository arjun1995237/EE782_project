# EE782_project-December 2020

colab file can be opened using the following link:		https://colab.research.google.com/drive/17sxP2NJ0DtkNnnpBRf4OWLLYbAC5j1wF?usp=sharing


Image denoising using convolutional autoencoders with skip connections

X-Rays, MRI, CT, ultrasound are susceptible to noise and its important to
denoise these images before doing any further analysis. Deep learning based
image denoising methods have outperformed all conventional denoising method.
These networks are less restrictive to specification of noise generative process.
Here we used small sample size and used convolutional denoising autoencoder
with concatenation of feature maps from encoder to decoder side (similar to
UNET). We used heterogeneous medical data for increasing the sample size.
We also confirmed that, we can recover signal even when the noise levels are
very high, at the point when other methods (conventional methods) will fail


Dataset-
Here we used three different datasets. They include 116 dental X-Ray images,
594 chest X-Ray images and 320 head X-Ray images. We mixed chest X-ray
and dental X-ray images into a single dataset containing 710 images . These 710
images were split at 0.8:0.2 as training:validation. Noisy version of the training
data was given as the input to my model and the corresponding noiseless ones
were taken as ground truth. We used head X-ray to test how well the model
worked ( data from some other distribution).
