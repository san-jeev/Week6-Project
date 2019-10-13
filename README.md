# Week6-Project
Week6 Project - GAN
- Instantiate a class called GAN with Image shape (28,28,1); Use Adam optimizer and initialize it
- Instantiate the discriminator by building and compiling the discriminator
- Instantiate and build the generator using build_generator
- Get the generated image with noise as input
- Take the generated images as input for Discriminator to determine validity
- Combine the stacked Generater and Discriminator models. For the combined model only train the generator to fool the discriminator
- Build Generator through Sequential model layer by layer (Dense, ReLU, BatchNormalization, Activation tanh) and reshape; Print Model Summary; Add some noice to model
- Build Discriminator through Sequential model layer by layer (Flatten, Dense, ReLU, Activation Sigmoid) and reshape; Print Model Summary; Given an input image from generator, the Discriminator outputs the likelihood of the image being real or not
- Pit the two models (Generator and Discriminator) against each other by defining a training function, loading the data set, re-scaling training images and setting the ground truths.
- Loop through a number of epochs to train Discriminator by first selecting a random batch of images from true dataset, generating a set of images from Generator, feeding both set of images into Discriminator, and finally setting the loss parameters for both the real and fake images, as well as the combined loss.<br>
- Train Generator, by setting the input noise and ultimately training the Generator to have the Discriminator label its samples as valid by specifying the gradient loss.
- Keep track of training process by printing the progress and save the sample image output depending on the epoch interval specified. When the specific sample_interval is hit, call the sample_image function and save images for viewing
- Call original GAN class and pass in the expected parameters

<img src="Figure-1.png" width=1000><br><br>
<img src="Figure-2.png" width=1000><br><br>
<img src="Figure-3.png" width=1000><br><br>
<img src="Figure-4.png" width=1000><br><br>
<img src="Figure-5.png" width=1000><br><br>
<img src="Figure-6.png" width=1000><br><br>
<img src="Figure-7.png" width=1000><br><br>
<img src="Figure-8.png" width=1000><br><br>
<img src="Figure-9.png" width=1000><br><br>
<img src="Figure-10.png" width=1000><br><br>
<img src="Figure-11.png" width=1000><br><br>
<img src="Figure-12.png" width=1000><br><br>
<img src="Figure-13.png" width=1000><br><br>
<img src="Figure-14.png" width=1000><br><br>
<img src="Figure-15.png" width=1000><br><br>
