### A Simple PyTorch implementation of GradCAM and GradCAM++ for example PET image

This repository contains a simple PyTorch implementation of GradCAM [1], and GradCAM++ [2] for example PET image [3].

The following repository re-uses the code by [1Konny](https://github.com/1Konny) from: https://github.com/1Konny/gradcam_plus_plus-pytorch.
It was the only simple working example on the use of GradCAM I was able to find on the Internet.
I decided to create a new repository (copy it) instead of forking the existing one because this way
it is easier to manage features such as repository title, issues, etc.

My modification is that I fixed one [error](https://github.com/1Konny/gradcam_plus_plus-pytorch/issues/10), and
I used a PET image from [this article](https://www.oatext.com/pet-myocardial-perfusion-imaging-in-the-assessment-of-coronary-artery-disease-the-basics.php) [3]
this example. Additionally, I made some changes to the README for better
readability.

<p align="center">
<img src=assets/readme.png>
</p>

### Supported `torchvision` models

- alexnet
- vgg
- resnet
- densenet
- squeezenet

### Usage

Please refer to `example.ipynb` for general usage and refer to documentations of each layer-finding functions
in `utils.py` if you want to know how to set `target_layer_name` properly.

### References

[1] Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization, Selvaraju et al, ICCV, 2017 <br>
[2] Grad-CAM++: Generalized Gradient-based Visual Explanations for Deep Convolutional Networks, Chattopadhyay et al, WACV, 2018 <br>
[3] Prieto-Vargas, V., Bautista-Prez-Gavilan, A., Lucio-Báez, O.E., Sierra-Poblete, S. and Gurrola-Luna, H., 2022. PET-Myocardial Perfusion Imaging in the Assessment of Coronary Artery Disease: the basics. Clin Res Trials, 8.
