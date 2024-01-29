## 1. Introduction
This repository motivates to introduce and run Pedersen commitment. The Pedersen commitment is based on ECDSA bilinear pairing. The ECDSA bilinear pairing has certain cryptographic properties like additive homomorphism, from which we are able to do Pedersen commitment verification.   

<br>

## 2. Requirements

**Requirement 1.** setup a conda environment for python 3.9,
```shell
$ conda create -n pedersen python=3.9
$ conda activate pedersen
(pedersen) $
```

**Requirement 2.** install the dependent library 3.20.0,
```shell
(pedersen) $ pip install pycryptodome==3.20.0
```

<br>

## 3. Run
Run the source code,
```shell
(pedersen) $ python main.py
```




<br>

## Acknowledgement
This repo was done when working with ASTRI Security Lab, Hong Kong Applied Science and Technology Research Institute.


<br>

## Reference
[1. Source Code of Pedersen Commitment] https://asecuritysite.com/encryption/ped