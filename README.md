# Dog_Breed_Classifier- Feedback and insights collected from reviews, forums & slack channel

* how to generate the bottleneck features yourself. See https://blog.keras.io/building-powerful-image-classification-models-using-very-little-data.html under the heading " Using the bottleneck features of a pre-trained network: 90% accuracy in a minute" on how to do this with Keras.
* After that you should be ready to take part in one of the playground competitions on Kaggle like https://www.kaggle.com/c/dog-breed-identification and https://www.kaggle.com/c/plant-seedlings-classification. Check out the kernels to learn techniques and tricks from other people and see if you can get a top leaderboard score!

https://www.superdatascience.com/opencv-face-detection/
http://www.bogotobogo.com/python/OpenCV_Python/python_opencv3_Image_Object_Detection_Face_Detection_Haar_Cascade_Classifiers.php

Considerations for CNN architecture
* https://keras.io/layers/normalization/to further improve the performance of your model. BatchNorm avoids "internal covariate shift" as it minimises the effect of weights and parameters in successive forward and back pass on the initial data normalisation done to make the data comparable across features as explained https://www.quora.com/Why-does-batch-normalization-help

* https://datascience.stackexchange.com/questions/20104/how-to-improve-my-test-accuracy-using-cnn-in-tensorflow

Considerations for number of epochs used to train the algorithm
To not worry about manually tuning the number of epochs or worry about overfitting, I recommend using an early stopping callback that Keras provides. Early stopping will automatically end training based on some specified rule, such as the accuracy not improving after a certain number of epochs. Take a look at https://keras.io/callbacks/ 

Overview of Gradient descent optimizers http://ruder.io/optimizing-gradient-descent/index.html
