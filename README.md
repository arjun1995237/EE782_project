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
