# Automatic Background Color Detection for Images

Have you ever wondered how Instagram Stories automatically select a background that complements the added image? This project explores two techniques to detect a suitable background for an input image.

## Approach 1: RGB Matrix Analysis

In this method, the RGB matrices of the image are separated. A frequency count is performed for each pixel value in the individual RGB matrices using the Counter() function. The top 10 most frequent values are selected, and their average is calculated to obtain the resultant pixel value. Finally, a blank image is generated using np.zeros() and filled with the determined background color to showcase the final result. While a straightforward approach, it yields results in just 40 lines of code.

## Approach 2: K-Means Clustering

The second technique involves applying the K-Means Clustering algorithm to the RGB values of the image. This identifies clusters of different color sets within the image. Subsequently, a frequency count is performed, and the background color is determined. This method leverages unsupervised machine learning and finds applications beyond background color detection, extending to tasks like image segmentation.

### Sources and References:

1. [Using K-Means Clustering on Image](https://towardsdatascience.com/color-identification-in-images-machine-learning-application-b26e770c4c71)
2. [Using Separate RGB Values](https://medium.com/generalist-dev/background-colour-detection-using-opencv-and-python-22ed8655b243)



This work was carried out by Mohammad Adnaan.

- [LinkedIn](https://www.linkedin.com/in/mohammad-adnaan-51272024a/)
- [GitHub](https://github.com/mohd-adnaan)

Feel free to explore the provided code and adapt it for your projects. Happy coding!