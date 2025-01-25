# Unsupervised Anomaly Lung Detection

<p align="justify">
Abnormalities localization in medical imagery has been a quiet challenge, as it requires pointing out the area accurately, preventing miss-diagnosis. In addition, several methods were once designed for a classification-only task which was limited to predicting labels of the presence of diseases from the input image, trained with sufficient data, yet it does not satisfy the requirement of visualizing tasks in the biomedical field nor does the medical field have sufficient labeled data samples, which gives birth to U-Net as a model to learn semantic segmentation of the disease area with minimal data. However, the problem of anomaly localization still exists in several approaches that have been proposed to overcome the problem of labeled data scarcity in the medical field, which mainly use a supervised approach by using disease labels and using part of the architectures to get the baseline reasoning for the model to predict an image to a specific label or through semantic segmentation using U-Net
</p>

![Architecture](/image/VAE-GAN.png)

![Result](/image/VAEGAN%20Result.png)


|              Model            |AUROC | DICE |Inference|
| ----------------------------- | ---- | ---- | ------- |
| Convolutional U-Net           | 0.53 | 0.16 | 3.89 ms |
| Variational Autoencoder (VAE) | 0.65 | 0.23 | 1.57 ms |
| VAEGAN                        | 0.60 | 0.21 | 2.85 ms |
