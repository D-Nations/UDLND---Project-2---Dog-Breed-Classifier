# UDLND---Project-2---Dog-Breed-Classifier

CNN Project to classify dog breeds and apply the model to images of people.  There were a lot of things in this project that I learned from.  This was the first project that I trained on my personal machine, so I spent a few hours trying to get the right libraries installed to make use of the video card that I had bought for machine learning earlier this year (RTX 2070).  Then I had to spend time adjusting the code to make it work on updated libraries.  Once all that was done, I had a little more freedom to play around with other tools.  Ultimately, I finished the project on the Udacity workspace because I thought there was still a problem with the Cuda drivers, but it turns out I was just using the default Windows 10 performance monitoring window to check if it was working, and you have to actually select Cuda to see GPU usage for training.

Here's a rundown of what I learned in this project:
* Face detection with OpenCV
* Face detection with dlib
* Cuda libraries and drivers
* PyTorch libraries that speed up processing on Intel CPUs
* Customized Dataloaders and Transforms
* Custom checkpoints for training
* Transfer learning witch VGG16
* Exposure to various publicly available pre-trained CNNs
* Freezing weights on some layers and customizing the classification layer
* Using a classifier on different types of images than what the model was trained on for fun

## Training the Model

Extract the Data archive files into the same directory as the model.

## Thoughts

This took a long time for me to complete but I found the whole experience very rewarding.  I hope and expect to use everything I learned from this project.  It took a lot of my alloted GPU time on the Udacity workspace to finish the project and get the model above 60% accuracy, but when I got the hang of the hyperparameters the solution that I ended up with took very little time to train.  The two biggest lessons I took from this are:
* If you're chasing down an error you don't understand, the location of the error is probably the biggest clue.  Chase down everything related to that until you can't anymore.
* It's possible to waste extreme amounts of time if hyperparameters are even slightly off.  Make sure to get those right before you invest too much in training.
