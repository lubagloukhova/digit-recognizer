# digit-recognizer


The two notebooks detail work in training four different Keras CNN models with two additional modifications -- learning rate annealing and data augmentation. We show how data augmentation aids in reducing overfitting (evidenced by instances where training accuracy exceeds validation accuracy. We also show how a higher validation accuracy score is achieved when we implement adaptive learning rate that decreases by a factor of two everytime accuracy is non-decreasing after 3 epochs (implemented via Keras ReduceLROnPlateau function from Keras.callbacks). In 3 our of 4 cases (i.e. most model architectures tested) the combination of data augmentation and learning rate annealing lead to improved validation accuracy. The fourth case's counter intuitive result of a model architecture performing best with neither data augmentation not learning rate annealing can be attributed to randomness. 


## The two notebooks: 
- [cnn_kerasTF_Model1.ipynb](https://github.com/lubagloukhova/digit-recognizer/blob/master/cnn_kerasTF_Model1.ipynb): Details training & analysis of a modle architecture featured in a top kaggle kernel, with an without data augmentation and learning rate annealing.
- [cnn_kerasTF_compare4.ipynb](https://127.0.0.1:8157/notebooks/digit-recognizer/cnn_kerasTF_compare4.ipynb): Details training & analysis of a three additional model architectures, each with an without data augmentation and learning rate annealing.



## Discussion of Architecture performance: