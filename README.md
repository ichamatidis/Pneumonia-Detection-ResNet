# Pneumonia detection
Finetune Resnet52 and VGG16 to detect pneumonia(viral or bacterial). The problem is tackled by splitting it into 2 subproblems, so it's tackled as 2-class problem.
1. Helthy vs Pneumonia person, all the healty images vs all the pneumonia images(viral and bacterial)
2. Viral pneumonia vs Bacterial pneumonia, train the model to detect if it's viral or bacterial pneumonia

The contained images are the class activation maps from the last convolutional layer of VGG16, they are on top of the original
X-Ray, so we can see where the network "saw"  the pnaumonia which provides a little explainability.

The dataset is from Kaggle and can be found here:
https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia
