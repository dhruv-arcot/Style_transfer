# Style_transfer

In this project we take the style of one particular image, which includes its features like brush stroke, highlights and palette, onto another image. 

This is performed using deep learning and the capabilites of neural networks. 

We initally diffrentiate on how different the 2 images are and see how much of the particular style we can apply to our target or output image without it being too distant from the content image. We’ll transform the base input image by minimizing the content and style distances (losses) with backpropagation, creating an image that matches the content of the content image and the style of the style image.


In the process, we will build practical experience and develop intuition around the following concepts

  Eager Execution 
  Using Functional API to define a model 
  
The steps followed for the same include: 

  Visualize data
  Basic Preprocessing/preparing our data
  Set up loss functions
  Create model
  Optimize for loss function
  
Content Loss calculation

Our content loss definition is actually quite simple. We’ll pass the network both the desired content image and our base input image. This will return the intermediate layer outputs (from the layers defined above) from our model. Then we simply take the euclidean distance between the two intermediate representations of those images.

Style Loss Calculation
Computing style loss is a bit more involved, but follows the same principle, this time feeding our network the base input image and the style image. 

Papers and algorithms reffered:
  https://arxiv.org/abs/1508.06576
  
  
  

