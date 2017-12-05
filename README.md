I have implemented some easy to understand data augmentation techniques which might help in generating realistic scenarios and datasets in problems where the size of the training dataset is relatively small and high performance is required.

The idea behing data augmentation is that by introducing the network to such augmenteded images, the neural network can be made invariant to small changes like mirroring, zoomed out / in images, small jitters in colors, etc which might occur in a realistic distribution for a particular computer vision problem. 

But one of its major uses is also to increase the size of the training dataset in such a way that the information learnt by the network is not duplicated given that new training images are not added explicitly.

I have implemnted 3 popular techniques namely:

1) Mirroring of an image
2) Random Cropping
3) Fancy PCA as mentioned in Krizhevsky et.al. https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks

I have also provided explanations in the comments for each technique, which are very easy to understand.

Note: For random cropping I have used the excellent technique mentioned in this answer https://stackoverflow.com/questions/34574714/random-cropping-data-augmentation-convolutional-neural-networks


Also note that Data Augmentation is a good technique to combat overfitting but not good enough ,as the synthesized images still have a high amount of correlation
