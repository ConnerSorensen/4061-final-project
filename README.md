## Fall 2020 INET 4061 Final Project - University of Minnesota
#### Collaborators: Conner Sorensen, Elias Noyes, Josh Gresko, Tajudin Aliy

This project was an exploration of computer vision and transfer learning. We trained a computer vision model on the MNIST handwritten digit database and attempted to apply that model to detecting speed limits. It never achieved great performance, approaching 10.5% accuracy at its best.

Upon reflection we realized many problems that could be addressed. First and foremost our application had no way to assess the feasibility of a result, "speed limits" with 10 digits were accepted without question. Another problem was that it would frequently find one digit, usually a 0, but not the other, or would recognize parts of digits as digits in their own right (e.g. detecting 8 as two stacked 0s). This was likely a side effect of the training set we used, as 0s on road signs look much more similar to handwritten 0s than other digits do.

&nbsp;

We used [Detectron 2](https://github.com/facebookresearch/detectron2), a PyTorch based object detection platform, to implement our model.

MNIST source: http://yann.lecun.com/exdb/mnist/

YYMNIST source: https://github.com/YunYang1994/yymnist

Test dataset source: https://www.kaggle.com/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign

&nbsp;

The IPython notebook does not run as is. The model was stored pre-trained in a Google Drive account of one of the collaborators, but that is inaccessible now.
