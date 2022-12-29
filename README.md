# Image-Compression-Using-PCA

Normally images have a lot of pixels to retain their clarity, but that significantly increases its size and slows down the performance of the system when it has to process multiple images. To overcome this situation we can use the dimensionality reduction technique which comes under Unsupervised Machine Learning.

Principal component analysis, or PCA, is a dimensionality-reduction method that is often used to reduce the dimensionality of large data sets, by transforming a large set of variables into a smaller one that still contains most of the information in the large set.
Reducing the number of variables of a data set naturally comes at the expense of accuracy, but the trick in dimensionality reduction is to trade a little accuracy for simplicity. Because smaller data sets are easier to explore and visualize and make analyzing data much easier and faster for machine learning algorithms without extraneous variables to process.

This is the image I used for compressing.

![download (1)](https://user-images.githubusercontent.com/96775630/209915815-18f77221-4f95-49bd-98d3-779a656a8bc1.png)


We will first split the image into the three channels (Blue, Yellow, and Red) and then and perform PCA separately on each dataset representing each channel and will then merge them to reconstruct the compressed image. Hence, if our colored image is of shape (m, n, 3), where (m X n) is the total number of pixels of the image on the three channels (b, y, r).

Compressed image is shown below:

![download (2)](https://user-images.githubusercontent.com/96775630/209915996-edd48f71-dbb7-4abe-bfe2-dbd43ff97f77.png)

The compressed image is very similar to that of the original one although we have reduced the dimension individually for each channel to only 50 from 2312.
