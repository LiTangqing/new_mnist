# new_mnist

Auto parse the original mnist database(http://yann.lecun.com/exdb/mnist/) and construct new dataset. 

The MNIST database is a dataset of handwritten digits. It has 60,000 training
samples, and 10,000 test samples. Each image is represented by 28x28 pixels, each
containing a value 0 - 255 with its grayscale value.

This repo is adapted from https://github.com/datapythonista/mnist

### Usage
To construct new set with particular composition (e.g. 20 images of 1s and 100 images of 2s), simply use 

```
import mnist

imgs, labels = mnist.customise_dataset({1:20, 2:100})
```

The dataset is downloaded and cached in your temporary directory, so, calling
the functions again, is much faster and doesn't hit the server.



See example notebook for details.
