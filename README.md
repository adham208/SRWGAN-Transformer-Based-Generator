
# SRWGAN (Super Resolution Wasserstein) GAN


This is an implementation of Super resolution GAN using a transformer as the generator

## What Does a GAN consist of ?
A GAN consists of 2 main components 

1 - Generator: The generator's job is to create data that resembles real data. It starts by taking random noise as input and generates an output, usually an image or some other form of data. The goal of the generator is to improve over time and produce more convincing data.

2 - Discriminator: The discriminator’s task is to distinguish between real data (from the actual dataset) and fake data (produced by the generator). It outputs a probability indicating whether the data is real or fake.

The Generator's goal is to "[Deceive](https://dictionary.cambridge.org/dictionary/english/deceive)" the discriminator (wow deceive is actually the exact word to describe such a thing :D) As the training progresses, the generator becomes more skilled at creating realistic data, and the discriminator becomes better at distinguishing between real and fake data. This "cat-and-mouse" dynamic is what drives the improvement of both models.
the generator’s outputs are usually very poor, but over time, as it learns from the feedback provided by the discriminator, it begins to produce increasingly realistic data. The discriminator also improves by learning to identify even the subtle differences between real and generated data, making the entire process a challenging back-and-forth.

# So what's so special about this SRWGAN ?

A Transformer-based Generator to upsample and refine low-resolution images.

# Dataset

We Used the DIV2K dataset it had only high resolution so we downscaled the images in order to get some low resolution images so we can upscale them afterwards.


# Results
DISCLAIMER : These Result were limited due to the limitation of the resources.

PSNR (Peak Signal-to-Noise Ratio) -> 9.4137
SSIM (Structural Similarity Index Measure) -> 0.1004


![image](https://github.com/user-attachments/assets/a9d55abb-3a77-42c2-83d5-e91691698fba)



# improvements

It could've been good if we had some more resources to Train the Model even more
