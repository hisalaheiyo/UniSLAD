The architectural details of the Wide-ResNet-50 layers utilized for feature extraction are as follows:
| block1          | block2                        | block3                                    | block4    |
|-----------------|-------------------------------|-------------------------------------------|-----------|
| layer1.0        | layer2.0                      | layer3.1                                  | layer4.0  |
| layer1.1        | layer2.1                      | layer3.2                                  |           |
| layer1.2        | layer2.2                      | layer3.3                                  |           |
|                 | layer2.3                      | layer3.4                                  |           |
|                 |                               | layer3.5                                  |           |

Hyperparameter settings on the MVTec LOCO AD dataset:

| Category             | Sampling Rate in ViT | Sampling Rate in ResNet | $w_i$  | $w_{ig}$ |$w$  | Layer in ViT |
|----------------------|----------------------|-------------------------|------|------|------|--------------|
| Breakfast Box        | 0                    | 0.01                    | 0.2  | 0.6  |  0.5  | 12           |
| Juice Bottle         | 0.65                 | 0.01                    | 0.6  | 0.2  |  0.6  | 10           |
| Pushpins             | 0.4                  | 0.05                    | 0.3  | 0.3  |  0.1  | 12           |
| Screw Bag            | 0.95                 | 0.05                    | 0.7  | 0.9  |  0.5  | 12           |
| Splicing Connectors  | 0.4                  | 0.1                     | 0.7  | 0.9  |  0.6  | 9            |

Specifically, ViT denotes ViT-B/16, ResNet denotes Wide-ResNet-50.
