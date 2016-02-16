
ConvNet on mobile metadata
=====================================
This repository contains the Caffe definition files used for our paper 'Using Deep Learning to Predict Demographics from Mobile Phone Metadata' that is submitted to KDD 2016. Below is a short description on how to use our ConvNet architecture in Caffe.

Prepare the Dataset
-------------------
First you will need to output the fitting 'week-matrix' data representation. It is implemented in the bandicoot toolbox, which can be found at bandicoot.mit.edu/. The data then needs to be normalized and outputted to a fitting Caffe format such as HDF5. You should add the relevant paths to the datasets at the top of the prototxt files under `source`.

Setting Hyperparameters
-------------------
We use Bayesian optimization to find a good set of hyperparameters for our ConvNet (see the paper for more details). Our Caffe definition files does therefore not include these parameters. To use our ConvNet architecture you must therefore insert these hyperparameters into the prototxt files at the lines marked with "<insert>".

Training and Testing
--------------------------------------
You should be good to go once the solver.prototxt and prototxt files for the architecture have been adjusted according to your hyperparameters and file structure. Any version of Caffe released after September 1, 2015 should be able to use the ConvNet architecture. Examples of how to train and run a model in Caffe can be found at https://github.com/BVLC/caffe.

Pretrained Models
--------------------------------------
These will be uploaded soon.

Feel free to send any questions to bfelbo@dtu.dk.
