This repo is a simple example to load data using TensorFlow Datasets and evaluating and training a Keras model using Keras Generators.

There is room for speeding up or pipelining the loading, so please feel free to create a Pull request!

# Downloading ImageNet
TensorFlow Datasets expects ImageNet to be downloaded to a specific directory in your home, so you need to follow these steps for the script to run:
1. Create the directory where the ImageNet should reside:
```
mkdir -p ~/tensorflow_datasets/downloads/manual/imagenet2012
```

2. Visit [Image-Net Downloads page](http://image-net.org/download-images) and create a user account with Image-Net if you haven't done so already.

3. Go to [Download links to ILSVRC2012 image data](http://www.image-net.org/challenges/LSVRC/2012/nonpub-downloads) page.

4. Download `ILSVRC2012_img_train.tar` from [Training images (Task 1 & 2)](http://www.image-net.org/challenges/LSVRC/2012/nnoupb/ILSVRC2012_img_train.tar) to `~/tensorflow_datasets/downloads/manual/imagenet2012`

5. Download `ILSVRC2012_img_val.tar` from [Validation images (all tasks)](http://www.image-net.org/challenges/LSVRC/2012/nnoupb/ILSVRC2012_img_val.tar) to `~/tensorflow_datasets/downloads/manual/imagenet2012`

# Getting Started
1. Clone the repo:
```
git clone https://github.com/mostafaelhoushi/keras-imagenet.git
```

2. cd into the directory
```
cd keras-imagenet
```

3. [Recommended] The code has been tested on specific versions of Keras, TensorFlow, and TensorFlow Datasets, so we recommend to install those specific versions in a local environment using `virtualenv`:
```
virtualenv venv
source venv/bin/activate
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
