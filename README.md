# Learning Deep Learning By Doing 2 
This is the second self assigned deep learning project. In this project, I will use the Stochastic Weight Averaging (SWA). <br>
## Stochastic Weight Averaging
SWA is an optimization technique that improves the generalization of the deep neural network. It can be used with any optimizer (SGD, Adam, RMSProp,..) and it comes to play after 75% of the training usually after the standard learning rate decay to average the weights in the last 25% of the training.<br>
[For more details](https://pytorch.org/blog/stochastic-weight-averaging-in-pytorch/) 
## Transfer Learning 
It is a very good practice to test out the state of art models and adapt them to your specific dataset by adapting the fully connected layers and see if you can get good results out of pre-trained models.
### Finetuning the convnet
Load a pretrained model and reset final fully connected layer.
### ConvNet as fixed feature extractor
Here, we need to freeze all the network except the final layer. We need to set ``` requires_grad = False ``` to freeze the parameters so that the gradients are not computed in ```backward()```.
[For more details](https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html)


