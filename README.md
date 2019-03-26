This repo is a simple example to load data using TensorFlow Datasets and evaluating and training a Keras model using Keras Generators.

There is room for speeding up or pipelining the loading, so please feel free to create a Pull request!

#Getting Started
1. Clone the repo:
```
git clone https://github.com/mostafaelhoushi/keras-imagenet.git
```

2. cd into the directory
```
cd keras-imagenet
```

3. The code has been tested on specific versions of Keras, TensorFlow, and TensorFlow Datasets, so we advise to install those specific versions in a local environment using `virtualenv`:
```
virtualenv venv
source bin\activa
pip install keras==2.2.4
pip install tensorflow==1.13.1
pip install tensorflow-datasets==1.0.1
pip install pillow
pip install opencv-python
```

4. Run the example:
```
python imagenet_mobilenet.py
```
