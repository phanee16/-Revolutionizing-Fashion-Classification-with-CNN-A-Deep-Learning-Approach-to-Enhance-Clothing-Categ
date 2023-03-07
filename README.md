# Image Classification using Convolutional Neural Networks
![image](https://user-images.githubusercontent.com/47351536/223467909-0909059e-26af-4a3d-b940-cac1a4c233d4.png)

First, the necessary libraries are imported, including Pandas, NumPy, Matplotlib, Seaborn, TensorFlow, and Keras. Then, the Fashion-MNIST dataset is loaded and divided into training and testing sets. The distribution of the labels (clothing categories) in both sets is plotted using countplots from Seaborn library.

Next, the images and their corresponding labels are displayed using Matplotlib. The data is preprocessed by reshaping the image data to 4D and scaling the pixel values between 0 and 1. The labels are converted to categorical format using the to_categorical() function from the TensorFlow Keras utility library.

Finally, a CNN model is created using the Sequential API of Keras. The model consists of 5 layers - 3 convolutional layers and 2 dense layers. The convolutional layers use different numbers of filters and kernel sizes, followed by average pooling layers. The dense layers use a ReLU activation function and dropout regularization to prevent overfitting. The model is then compiled and trained on the training set using the Adamax optimizer and categorical cross-entropy loss. The training process is monitored using the accuracy metric, and early stopping is used to prevent overfitting.

The validation accuracy and training accuracy over epochs are plotted using Matplotlib to evaluate the performance of the model.
![image](https://user-images.githubusercontent.com/47351536/223468022-e3351af0-c663-4ebe-9299-c11c24042c25.png)

