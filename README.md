# neuralNetwork_imgClassification
This project demonstate how we can use convolution network to classify images, using the MNIST dataset we'll calssify images of number to the matching number category,
in simple terms a image of and 8 number will be classified as and 8 value.

## Workflow
- Data preperation
- Model building and training
- Evaluate models
- Showing the models prediction and activation maps of the convolotion layers.

## Models
- m1 - no hidden layers at all
- m2 - two hidden layers (no convolution)
- m3 - convolution network with a single covolotion layer and a two maxpools and linear layers
- m4 - same as m3 but with differnt sizes channelsSS
- m5 - m3 with a higher drop rate
- m6 - m4 with higher drop rate

reminder -> drop rate is the precentage of random neurorns that won't participate in training (different ones for each epoch)

## Resuslt
For each model we preduce a prediciton and see example where the predictions wer'e wrong.
For a network with a convolotion layer we plot the activation map that is created in the procces.


## Theory on one leg
The idea is to embbed the data of the pixcels of the input in such a way that our network could classify it a number, to do so we go through the image with fillters that samples the image.
One way of looking at it that a certain flitter is incharge of recognizing a particular pattern in the image such a a right egde then deeper in the network layers can represent combination of thouse founded elements, even though it's not practical to try and follow the roll of each fillter in deeper networks the idea still holds.
