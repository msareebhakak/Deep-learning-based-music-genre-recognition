## Music-genre-recognition-using-Keras
Deep-learning based approach for music genre prediction

This a music genre prediction model built using Keras-TensorFlow. This repository has 2 model architectures, one with CRNN network and another with parallel CNN-RNN model

* CRNN-model --> This model has a serial connection between CNN and RNN. We do a 1-D convolution, 1-D max pooling and batch normalization and feeds this feature vector to the RNN to get temporal features. The performance on of this model is rather unpredictable and more often than not, lower accuracy than 50%. 

* Parallel CNN-RNN model --> This model feeds the same mel-spectrogram of the audio track into the CNN and RNN. The CNN extracts spatial features with 2-D convolution, max pooling and batch normalization. The RNN extracts the temporal features from the same mel-spectrogram and outputs of these two are combined and sent to a fully connected network for final processing and prediction.
