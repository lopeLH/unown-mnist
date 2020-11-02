
# Unown-MNIST  <img src="https://github.com/lopeLH/unown-mnist/blob/main/doc/transition.gif" width=70>

`Unown-MNIST` is a dataset of artificially augmented unown pokemon images consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 28 classes. After so many years, MNIST has become kind of boring. While `Unown-MNIST` is certainly too easy to be taken seriously as a benchmarking dataset, at least can serve as an amusing sanity check for new algorithms.

Here's an example how the data looks:

<img src="https://github.com/lopeLH/unown-mnist/blob/main/doc/examples.png">

The dataset is distributed as a set of `uint8` serialized `numpy` arays:

| File        | Size           | Array dimension  | Description  |
| ------------- |:-------------:| -----:|-----:|
| [X_train.npy](https://github.com/lopeLH/unown-mnist/blob/main/X_train.npy)    | 45M  | `(60000, 28, 28)` | Training images|
| [X_test.npy](https://github.com/lopeLH/unown-mnist/blob/main/X_test.npy)      | 7,5M  |  `(10000, 28, 28)`   | Test images  |
| [Y_train.npy](https://github.com/lopeLH/unown-mnist/blob/main/Y_train.npy) | 469K      |    `(60000,)` | Training labels|
| [Y_test.npy](https://github.com/lopeLH/unown-mnist/blob/main/Y_test.npy) | 79K      |    `(10000,)` |Test labels|

To play arround with the augmentation steps applied to generate the dataset, and generate your own, have a look at [dataset_generation.ipynb](https://github.com/lopeLH/unown-mnist/blob/main/dataset_generation.ipynb).

FYI, I prepared this dataset to train a [GAN+CPPN](https://blog.otoro.net/2016/04/01/generating-large-images-from-latent-vectors/) and create cool unown transitions, and of course some brand new unowns:

<img src="https://github.com/lopeLH/unown-mnist/blob/main/doc/transition.gif">

<div class="row">
<img src="https://github.com/lopeLH/unown-mnist/blob/main/doc/generated1.gif" width=95> 
<img src="https://github.com/lopeLH/unown-mnist/blob/main/doc/generated2.gif" width=95>
<img src="https://github.com/lopeLH/unown-mnist/blob/main/doc/generated3.gif" width=95>
<img src="https://github.com/lopeLH/unown-mnist/blob/main/doc/generated5.gif" width=95>
<img src="https://github.com/lopeLH/unown-mnist/blob/main/doc/generated6.gif" width=95>
</div>
