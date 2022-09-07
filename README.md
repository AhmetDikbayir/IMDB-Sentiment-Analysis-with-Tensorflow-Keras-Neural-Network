# IMDB-Sentiment-Analysis-with-Tensorflow-Keras-Neural-Network

## Executive Summary¶ 

### About the dataset 

* IMDB movie review dataset was used in this project. 
* There are 25.000 training review and the same quantity of the test data. 
* The ready word index was used in this project. 

### Preprocessing the dataset 

* Convert the words to numeric thanks to word index by defining a function. 
* Added some html codes in this index. 
* Split the data train and test. 

### Build the Model  

* Sequential API was used.  
* Embedding Layer, after that Global Average Pooling, one hidden layer, two Dropout and Output Layer.  
* ReLu activation function was used in the hidden layer and Sigmoid activation function in the output layer.  
* Adam optimizer function and Binary crossentropy for loss and accuracy metrics was used in the model.  

### Evaluate the Model  

* After training this model, my model had overfitting.   
* To overcome this problem, I added Dropout layer aafter the Global Average Pool Layer with 0.2 percentage.   
* After added this layers, overfitting was still going on.   
* So, I added another Dropout Layer after the hidden layer.   
* When restart the analysis, I achieved reliable and acceptable results.  
* My model accuracy is .92 and validation score is .88.   
* I also visualize the train and test loss and accuracy.   
* Train dataset accuracy and test dataset do not differentiate significantly each other.  
* So it can be said that over-fitting cannot be seen.   
* All in all, I can say that my model is reliable model to determine the movie review.

