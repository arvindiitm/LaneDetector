Lane Detections using Semantic Image Segmentation with Atrous Convolution with a multi atrous rate and Boundary-aware Loss.This network uses Resnet as a backbone network for feature extraction. While Atrous Convolution with multiple atrous rates make model robust to multiples scales and also reduce the parameters for filters. Boundary Aware Loss can help the network to learn more hard regions from the data points.

# Prerequisite

    Python 3.5.x or 3.6.x
    Tensorflow 1.2 or higher
    Numpy, CV2, PIL, etc

# Usage 
     Run prediction.py by Python for predictions. You can modify model_dir, data_dir, output_dir to modify directories to predictions.
    
     Run train.py by Python to train network. You can modify several options in train.py. You can change the number of GPUs, Model directory, Dataset directory, etc by modifying flags options. 
    First, you have to convert your own dataset into tfrecord by utils/dataset_util.py. You can simply modify def make_***_tfrecord function in dataset_util.py to convert your dataset into tfrecord. And then, change model_dir, train_data, test_data in train.py, and run. You can change other variables to train your network like batch_size, max_iter, etc.


# reference
-  [Deep Residual Networks](https://github.com/KaimingHe/deep-residual-networks)
-  [DeepLabV3](https://arxiv.org/pdf/1706.05587.pdf)
-  [DrSleep/tensorflow-deeplab-resnet ](https://github.com/DrSleep/tensorflow-deeplab-resnet)
-  [rishizek/tensorflow-deeplab-v3-plus  ](https://github.com/rishizek/tensorflow-deeplab-v3-plus)
-  [tensorflow/models](https://github.com/tensorflow/models/tree/master/official)

