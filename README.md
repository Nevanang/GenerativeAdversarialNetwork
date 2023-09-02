# GenerativeAdversarialNetwork
DCGAN on CIFAR10
Cifar10 - https://www.bing.com/ck/a?!&&p=b20e3e76e2b029fcJmltdHM9MTY5MzYxMjgwMCZpZ3VpZD0zYjIzNTA5OS1lYzNmLTY4OTMtMjRkMi00MWQ1ZWQ5MzY5MWImaW5zaWQ9NTI1Nw&ptn=3&hsh=3&fclid=3b235099-ec3f-6893-24d2-41d5ed93691b&psq=cifar10&u=a1aHR0cHM6Ly93d3cudGVuc29yZmxvdy5vcmcvZGF0YXNldHMvY2F0YWxvZy9jaWZhcjEw&ntb=1
Discriminator and Generator architecture was used.

Generator is responsible for creating fake samples of data that look real using noise vectors(random inputs) to fool the discriminator
The discriminator will receive the fake generated samples along with real samples to determine which of them are authentic, its goal to successfully identify generated data as fake.
In this case, the split of real and fake samples were 50/50.

Uses deep convolutional neural networks than fully connected dense layers. Optimized with BatchNormalisation, ReLU for generator and LeakyReLU for discriminator and not using any pooling layers.

Done using Pytorch for fine tuned model while baseline was done on keras and evaluated with FID and Inception score.

