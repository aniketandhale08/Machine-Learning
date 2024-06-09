Pooling is performed in neural networks to reduce variance and computation complexity. 
Many a times, beginners blindly use a pooling method without knowing the reason for using it. Here is a comparison of three basic pooling methods that are widely used.

The three types of pooling operations are:

Max pooling: The maximum pixel value of the batch is selected.
Min pooling: The minimum pixel value of the batch is selected.
Average pooling: The average value of all the pixels in the batch is selected.
The batch here means a group of pixels of size equal to the filter size which is decided based on the size of the image. In the following example, a filter of 9x9 is chosen. The output of the pooling method varies with the varying value of the filter size.
