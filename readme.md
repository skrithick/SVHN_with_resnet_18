# Attempting to read numbers on houses from data collected from google streetview (SVHN dataset)

- ### Used a resnet 18 architecture [Source](https://www.researchgate.net/figure/Original-ResNet-18-Architecture_fig1_336642248) <br /><br /> ![arch](image.png)

- ### Training and Validation Loss <br /><br /> ![tvl](val_and_training_loss.png)

- ### Testing Loss <br /><br /> ![tl](testing_loss.png)

## Results (over 5 epochs):

| Dataset Split | Accuracy | Loss |
| :--- | :--- | :--- |
| Testing | 94.35% | 0.2054 |
| Validation | 94.04% | 0.2117 |
| Training | 95.35% | 0.1610 |

- We use resnet-18 with blocks sequenced as [64x2, 128x2, 256x2, 512x2]. This is so that we can have many layers for learning whilst not downsampling too quickly.
- When we downsample, we increase no. of channels to maintain computational efficienct and resource usage.