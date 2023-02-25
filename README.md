# neuralNetwork_imgClassification
This project demonstrate how we can use convolution network to classify images, using the MNIST dataset we'll classify images of number to the matching number category,
in simple terms an image of and 8 number will be classified as and 8 value.

## Workflow
- Data preparation
- Model building and training
- Evaluate models
- Showing the model's prediction and activation maps of the convolution layers.

## Models
- m1 - no hidden layers at all
- m2 - two hidden layers (no convolution)
- m3 - convolution network with a single convolution layer and a two maxpools and linear layers
- m4 - same as m3 but with different sizes channels
- m5 - m3 with a higher drop rate
- m6 - m4 with higher drop rate

reminder -> drop rate is the percentage of random neurons that won't participate in training (different ones for each epoch)

## Results
For each model we produce a prediction and see an example where the predictions were wrong.
For a network with a convolution layer, we plot the activation map that is created in the process.


<div style = "padding-bottom: 150; padding-top: 150;">
  <p align="center">
    <img src="/pic1.png"  style = " height: 350;  display:block; width:30%;"/>
   </p>
</div>


## Theory on one leg
The idea is to embbed the data of the pixcels of the input in such a way that our network could classify it a number, to do so we go through the image with fillters that samples the image.
One way of looking at it that a certain flitter is incharge of recognizing a particular pattern in the image such a a right egde then deeper in the network layers can represent combination of thouse founded elements, even though it's not practical to try and follow the roll of each fillter in deeper networks the idea still holds.
