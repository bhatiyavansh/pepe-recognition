My task was to create a classification neural network that can accurately classify whether an image contains Pepe the Frog or not.
My goal was to train a neural network model using this dataset and evaluate its performance in classifying new, unseen images.

I used a deep learning framework TensorFlow to create a convolution neural network

I first used the keras library to make a dataset from a local dir "data"
It already rescales the image to 256x256 pixels and creates a batch size of 32

Then we normalize the pixels to get the values close to each other by dividing each pixel value by 255

Then we split the dataset into the training,validation and test datasets in a ratio of 70-20-10 respectively
We use the training dataset to train the model, the validation set is used to check the accuracy while training the model to check for overfitting

Then we assign batches to each set 

Then comes the main part we use the sequential method of layers to build the model(runs thru the models in a sequential manner) '
then we use the following layers to create feature maps that as the training goes on, learns more and more abstract features about the image, thus making it easier for the computer to recognise
I used the following layers to make the most abstract and smallest datasets to create the most efficient and accuracte model possible


Then we compile the model using adam optimizer and use BinaryCrossentropy to minimize losses

Once we train the model, and log it so we can plot its accuracy/losses over time
then we just evaluate our metrics(all attachments enclosed)

Then we just test our model for unseen images.
