# GAN-Album-Cover
GANs for Album Cover Generation

> #### *Project is still on development stage*

### Summary
This project creates a Generative Adversarial Network (GAN) for album cover generation based on the Spotify dataset. It is based on [this paper](https://ryanmcconville.com/publications/AlbumCoverGenerationFromGenreTags.pdf) and the ultimate objective is to generate album images based on music genres.

There will be some intermediate steps on the process: 1 - Generate a data set 2 - Create an album image GAN 3 - Create a GAN that generates albums based on genre

## Notes

 - **According to this [sourse](https://machinelearningmastery.com/how-to-get-started-with-generative-adversarial-networks-7-day-mini-course/)** , there are seven best practices to consider when implementing your GAN model:

	1.  Downsample Using Strided Convolutions (e.g. don’t use pooling layers)
	2.  Upsample Using Strided Convolutions (e.g. use the transpose convolutional layer).
	3.  Use LeakyReLU (e.g. don’t use the standard ReLU).
	4.  Use Batch Normalization (e.g. standardize layer outputs after the activation).
	5.  Use Gaussian Weight Initialization (e.g. a mean of 0.0 and stdev of 0.02).
	6.  Use Adam Stochastic Gradient Descent (e.g. learning rate of 0.0002 and beta1 of 0.5).
	7.  Scale Images to the Range \[-1,1\] (e.g. use tanh in the output of the generator).

- Images from OMACIR dataset > Spotify dataset.
	- The authors of the [paper](https://ryanmcconville.com/publications/AlbumCoverGenerationFromGenreTags.pdf) initially downloaded the album covers from the OMACIR dataset and then found/downloaded the metadata of the albums from Spotify --> ~50k images
	- This project used the album images that were directly downloaded from Spotify --> ~30k images
	

