# Classification_Of_Facial_Expressions_Using_CNN
### An Investigation into the use of Convolutional Neural Networks to resolve facial characteristics

![Some of the faces in the database](https://www.wilmabainbridge.com/images/10kfacedatabase2.jpg)

The task was to use Convolutional Neural Network (CNN) analysis to classify the images by sex and by facial expression, using Keras with a TensorFlow back end. It was known from earlier studies that the VGG16 model had shown itself to be particularly effective at image recognition.

Thus the original gameplan was to train an image classifier on these 2,222 datapoints. The problem with this approach was that, with regard to facial expression, there was a significant class imbalance in favor of classes 0 (neutral) and 1 (happy).


The first remedy to this was to write a basic web scraper using Beautiful Soup, as will be shown later, in order to increase the numbers of the under-represented expression classes. Once the numbers of these classes had been increased, attempts were made to classify the images. Results were mixed, for either or both of two possible reasons:

* The disparate nature of the images scraped.
* Possibly inaccurate classifications by the survey respondents.


As such, the decision was made to trawl through the remaining 7,946 images that had not been pre-classified, and to find class exemplars among those to represent the under-balanced classes. Two of the classes, 'scared', and 'disgusted,' were dropped due to a dearth of available exemplars within the database. This resulted in a dataset of the following numbers, upon which the analysis began:


(0) Neutral

(1) Happy

(2) Sad

(3) Angry

(4) Surprised






This set of classes evolved throughout the course of the project, and some classes were later dropped, as will be explained later.
