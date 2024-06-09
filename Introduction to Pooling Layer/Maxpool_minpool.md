Pooling is performed in neural networks to reduce variance and computation complexity. 
Many a times, beginners blindly use a pooling method without knowing the reason for using it. Here is a comparison of three basic pooling methods that are widely used.

*The three types of pooling operations are:*

1. Max pooling: The maximum pixel value of the batch is selected.
2. Min pooling: The minimum pixel value of the batch is selected.
3. Average pooling: The average value of all the pixels in the batch is selected.

*Max Pooling*

Max pooling is a pooling operation that selects the maximum element from the region of the feature map covered by the filter. Thus, the output after max-pooling layer would be a feature map containing the most prominent features of the previous feature map. 
<img width="695" alt="Screenshot-2019-07-21-at-2 57 13-AM" src="https://github.com/aniketandhale08/Machine-Learning/assets/99685171/b87ccf1c-8ab9-443e-b552-2680396caa5e">

*Average Pooling*

Average pooling computes the average of the elements present in the region of feature map covered by the filter. Thus, while max pooling gives the most prominent feature in a particular patch of the feature map, average pooling gives the average of features present in a patch. 
<img width="695" alt="Screenshot-2019-07-21-at-3 05 56-AM" src="https://github.com/aniketandhale08/Machine-Learning/assets/99685171/d2b4aac0-f538-4502-95e0-2f8cd7d1838e">

The batch here means a group of pixels of size equal to the filter size which is decided based on the size of the image. In the following example, a filter of 9x9 is chosen. The output of the pooling method varies with the varying value of the filter size.

The operations are illustrated through the following figures.
![Figure_1](https://github.com/aniketandhale08/Machine-Learning/assets/99685171/a590ec01-b034-4cf1-9cad-17d9ec01921d)

We cannot say that a particular pooling method is better over other generally. The choice of pooling operation is made based on the data at hand. Average pooling method smooths out the image and hence the sharp features may not be identified when this pooling method is used.

Max pooling selects the brighter pixels from the image. It is useful when the background of the image is dark and we are interested in only the lighter pixels of the image. For example: in MNIST dataset, the digits are represented in white color and the background is black. So, max pooling is used. Similarly, min pooling is used in the other way round.
