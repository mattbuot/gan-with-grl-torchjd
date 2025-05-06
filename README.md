# GAN with Gradient Reversal Layer and Jacobian Descent

The idea is to train a GAN with a gradient reversal layer and to optimize it with Jacobian Descent using Torchjd.

## Training of GAN
```bash
$ python train_gan.py [options]
```

## Image generation from trained generator
```bash
$ python generate.py [options]
```

You can read help with `-h` option.

```bash
$ python gan.py -h
usage: gan.py [-h] [-b B] [-z Z] [-e E] [-r R] [--save_model]

Trains GAN

optional arguments:
  -h, --help    show this help message and exit
  -b B          batch size
  -z Z          dimension
  -e E          epoch
  -r R          result directory
  --save_model  save models
  
$ python generate.py -h
usage: generate.py [-h] -m M [-n N] [-z Z] [-r R]

Generates images randomly from trained generator model

optional arguments:
  -h, --help  show this help message and exit
  -m M        generator model file
  -n N        number of images to generate
  -z Z        dimension
  -r R        result directory
```
