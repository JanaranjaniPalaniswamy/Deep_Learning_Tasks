# Deep_Learning_Tasks
Deep Learning assignments using TensorFlow and Keras libraries - SS 2020.

#Tasks:

1. Simple regresion:
   In this task I revisited the mathematical background for a simple regression and covered it's practical implementation in Tensorflow 2. I also explored the phenomenon of overfitting and derived different regularizations from a probabilistic perspective. This exercise covers a very simple task with a very basic neural architecture. 
   
2. Age regression:
  In this part of the exercise I have applied the concept of regression to the problem of estimating the age of a person from his or her potrait. In this process I have seen how to load images from their filenames with the map function of the Dataset class. With this, images are loaded just in time as they are needed, which is beneficial while working with a large number of high resolution images that do not fit into your system memory all at once. I also used Keras in order to build our model from predefined layers to speed up develpment time and reduce possible error sources. I also observed that the labeling of the individual images is not optimal for our task, since it is rounded to integer ages and in the setting of regression I would rather like to have continuous age labels.
  
3. Classification task:
   In this exercise I have learned how to use Keras in order to quickly develop neural networks and train them on different data sets. I also explored how dropout can act as an effective regularization in order to mitigate overfitting. In order to evaluate a model on two different data sets in order to visualize the phenomenon of catastrophic forgetting, I implemented a custom callback that executed our required action at the end of every epoch. Besides that Keras offers many other ways to implement non standard layers/methods. Additionally I have explored a very basic transfer learning technique, i.e. fine tuning of pretrained models. For this I utilized the MobileNetV2 architecture that was trained on the ImageNet data set and fine tuned it on the Caltech 101 data set. The resulting model was simple to implement and fast to train, while it still achieved competetive results.

4. Text classification using RNN:
  This exercise classifies movie reviews as positive or negative using the text of the review. I utilizied RNNs for binary classification and IMDB dataset with movie reviews for traininig and testing. The training and testing sets are balanced, meaning they contain an equal number of positive and negative reviews. Used an embedding layer that stores one vector per word. When called, it converts the sequences of word indices to sequences of vectors. These vectors are trainable. After training (on enough data), words with similar meanings often have similar vectors. This index-lookup is much more efficient than the equivalent operation of passing a one-hot encoded vector through a tf.keras.layers.Dense layer. Perfomed this using RNN and LSTM layers and observed the performance diferences by visualizing the training plot.

5. DC GAN using mnist dataset:
  With this task created a DC GAN using generator and discriminator networks for the generation of MNIST digits.

 
            


