Pooling is performed in neural networks to reduce variance and computation complexity. 
Many a times, beginners blindly use a pooling method without knowing the reason for using it. Here is a comparison of three basic pooling methods that are widely used.

*The three types of pooling operations are:*

1. Max pooling: The maximum pixel value of the batch is selected.
2. Min pooling: The minimum pixel value of the batch is selected.
3. Average pooling: The average value of all the pixels in the batch is selected.

The batch here means a group of pixels of size equal to the filter size which is decided based on the size of the image. In the following example, a filter of 9x9 is chosen. The output of the pooling method varies with the varying value of the filter size.

The operations are illustrated through the following figures.
![Figure_1](https://github.com/aniketandhale08/Machine-Learning/assets/99685171/a590ec01-b034-4cf1-9cad-17d9ec01921d)

We cannot say that a particular pooling method is better over other generally. The choice of pooling operation is made based on the data at hand. Average pooling method smooths out the image and hence the sharp features may not be identified when this pooling method is used.

Max pooling selects the brighter pixels from the image. It is useful when the background of the image is dark and we are interested in only the lighter pixels of the image. For example: in MNIST dataset, the digits are represented in white color and the background is black. So, max pooling is used. Similarly, min pooling is used in the other way round.
