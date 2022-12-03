## Cosine Annealing
Cosine Annealing is a type of learning rate schedule that has the effect of starting with a large learning rate that is relatively rapidly decreased to a minimum value before being increased rapidly again. The resetting of the learning rate acts like a simulated restart of the learning process and the re-use of good weights as the starting point of the restart is referred to as a "warm restart" in contrast to a "cold restart" where a new set of small random numbers may be used as a starting point.
![image](https://user-images.githubusercontent.com/38180831/205463491-2813732d-7c82-47e5-a807-fa8a5add012c.png)
Here t is the number of weight updates of the network. This is called the cosine learning rate schedule with a warmup. The first phase until t ≤ T0 is called the warmup phase and the second phase where the learning rate decreases along a cosine is called the annealing phase.

## Dataset
The dataset used here is the [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html) which consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images. 

## Loss curves

The curve of the learning rate vs. loss is shown below. The minima of this plot is taken as the optimal learning rate.
![image](https://user-images.githubusercontent.com/38180831/205463701-e22f4afb-c97e-49ab-9ecf-2155b62c0995.png)

Plotting the Training loss, Training error and Learning rate as a function of the number of weight updates:
![image](https://user-images.githubusercontent.com/38180831/205463727-e02051c2-ccce-4dab-86be-fb40592763c3.png)

Plotting the Training Validation Loss and Training Validation accuracy as a function of the number of epochs:
![image](https://user-images.githubusercontent.com/38180831/205463741-b4163e50-247c-44cc-814c-fe9d6a7eceb0.png)
