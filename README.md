overview:::
This project implements a Convolutional Neural Network (CNN) for digit recognition using the SVHN (Street View House Numbers) dataset. The code loads,
preprocesses the dataset, defines a CNN model, trains the model, and evaluates its performance using various metrics.

Requirements::
To run this code, you will need:
Python 3.x,Libraries,NumPy,SciPy,Matplotlib,Seaborn,Scikit-learn,TensorFlow (Keras)

Dataset::
The dataset used in this project is the SVHN dataset, which can be found at SVHN Dataset. The training and testing data should be in .mat format.

Code Explanation::
Importing Libraries: The necessary libraries for data handling, visualization, and model building are imported.
The load_data function reads the dataset and returns image arrays and corresponding labels.Image arrays are reshaped to fit the CNN input format.
Labels are converted from a 2D array to a 1D array.Pixel values are normalized to a range of 0 to . Labels are converted into a one-hot encoded format.
Using ImageDataGenerator, various transformations are applied to training images to enhance model robustness.
A CNN model is defined with multiple convolutional and pooling layers, followed by dense layers and dropout for regularization. The model is compiled with the Adam optimizer and categorical cross-entropy loss function. The CNN is trained on the augmented dataset for a specified number of epochs. The model's performance is evaluated on the test dataset, with accuracy printed out.A classification report is generated, and a confusion matrix is plotted using Seaborn for better visualization of predictions. 

Conclusion::
This project demonstrates the implementation of a CNN for digit recognition using the SVHN dataset.
The model can be further improved by experimenting with different architectures, hyperparameters, and augmentation techniques.
