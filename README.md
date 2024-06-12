# Pytorch tutorials

Welcome to this repository where you can find **PyTorch tutorials! These tutorials can help anyone as they are very general and require no a priori knowledge of PyTorch nor deep learning.** However they were originally designed for our students in **[INF265: Deep learning](https://www4.uib.no/en/courses/INF265)**. INF265 is run by the University of Bergen (Norway) and is a part of the machine learning specialisation of the master program in informatics offered by the department of Informatics of the University of Bergen. I was fully responsible for the practical part of [INF265: Deep learning](https://www4.uib.no/en/courses/INF265), and you can see the entirety of the practical part of INF265 on [my corresponding repository](https://github.com/nglm/inf265).

## Content

1. **PyTorch datasets and transforms**
   1. The CIFAR Dataset
      2. Loading the CIFAR dataset in Pytorch
      3. Getting started with the CIFAR dataset
      4. Plot images
      5. Count how many samples there are for each class
   2. Transforms
      3. Convert an image into a PyTorch-friendly object
      4. Include the preprocessing step (transform operator) when loading the dataset
      5. Normalizing the dataset
2. **Define, train and evaluate a basic Neural Network in Pytorch**
   1. Loading data
       1. Loading CIFAR-10  (see previous tutorial)
       2. From CIFAR-10 to CIFAR-2
   2. Basic building blocks for neural networks in PyTorch
       1. The 'torch.nn' module and the 'torch.nn.Module' class
       2. Our network as a nn.Sequential object
       3. Pytorch notations and dimensions
       4. Inspecting a module object
   3. Training our model
       1. Training on CPU
       2. Training on GPU
3. **Define a custom deep Neural Network in Pytorch**
   1. .Loading data, training and measuring accuracy (see previous tutorial)
   2. Define a simple custom neural network
       1. Naive (but totally ok) method
       2. Using the functional API
       3. Train our custom network (as any other model)
       4. Measuring accuracy (as any other model)
   3. Going deeper: defining blocks of layers
       1. Using nn.Sequential
       2. Using a subclass of nn.Module
4. **Computational graph**
   1. MiniNet
   2. PyTorch's computational graph
       1. Weight and gradient values
       2. Updating weights
       3. Updating gradients
   3. Good to know
5. **Input and output shapes of convolutional neural network layers**
   1. A specific example
      1. Loading data
      2. Defining a convolutional neural network
   2. Figuring out shapes when stacking layers
       1. Shape of the data
       2. 1st layer: Convolution, [nn.Conv2d](https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html#conv2d)
       3. Intermediate layer: MaxPool, [nn.MaxPool2d](https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html#maxpool2d)
       4. 2nd layer: Convolution again
       5. 2nd Intermediate layer: MaxPool, [nn.MaxPool2d](https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html#maxpool2d)
       6. 3rd layer: Fully connected layer [nn.Linear](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html#linear)
       7. 4th layer: Fully connected layer [nn.Linear](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html#linear)