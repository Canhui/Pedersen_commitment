## 1. Introduction
This repository motivates to introduce and run Pedersen commitment. The Pedersen commitment (Pedersen 承诺) is based on ECDSA bilinear pairing. The ECDSA bilinear pairing has certain cryptographic properties like additive homomorphism, from which we are able to do Pedersen commitment verification.   

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
Secret value:    558045267788217253125593857129503771198756026678
p= 1158367283022461159590633765000078783673950159781
q= 2316734566044922319181267530000157567347900319563
g= 1670959692723208939270314333104457008202332655153
h= 2283916898129036336169835146345243390146861914555

Msg1: 1
Msg2: 2

c1,r1: 1486089786256113121040746209690183096221837214461 , 2256718608198722450494021155003652883309829684640
c2,r2: 759571960538886299715614947979389967197620978127 , 427743376760848238246259009909965696735156826500

We can now multiply c1 and c2, which is same as adding Msg1 and Msg2

Commitment of adding (Msg1+Msg2):        985974020805726589789752982524217159510497396398

Result of verifying c1:          True
Result of verifying c2:          True
Result of verify Msg+Msg2:       True
```



<br>

## Acknowledgement
This repo was done when working with ASTRI Security Lab, Hong Kong Applied Science and Technology Research Institute.


<br>

## Reference
[1. Source Code of Pedersen Commitment] https://asecuritysite.com/encryption/ped

[2. Chinese Explanation] https://blog.csdn.net/mutourend/article/details/93739575 

<br>

## Long-Term Support (LST) Log

[12 Mar 2024]: Repetable validation, succeed.

[31 Jan 2024]: Repetable validation, succeed.

[30 Jan 2024]: Repetable validation, succeed.
