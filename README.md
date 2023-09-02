# GenerativeAdversarialNetwork
DCGAN on CIFAR10

Discriminator and Generator architecture was used.

Generator is responsible for creating fake samples of data that look real using noise vectors(random inputs) to fool the discriminator
The discriminator will receive the fake generated samples along with real samples to determine which of them are authentic, its goal to successfully identify generated data as fake.
In this case, the split of real and fake samples were 50/50.

Uses deep convolutional neural networks than fully connected dense layers. Optimized with BatchNormalisation, ReLU for generator and LeakyReLU for discriminator and not using any pooling layers.

Done using Pytorch for fine tuned model while baseline was done on keras.

