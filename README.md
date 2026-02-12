# README

## Overview

The README provides some info on the topic learning from data provided as open learning from Prof. Abu Mostafa of Caltech Univ.

### References
- Caltech course for Learning from Data: https://work.caltech.edu/telecourse.html
- Youtube playlist for Learning from Data: https://www.youtube.com/playlist?list=PLD63A284B7615313A

## Details

### key concepts

- perceptron model

Takes attributes (x) and gives different weights (w) and adds in a linear form (e.g sum of x_i*w_i )

$$\left( \sum_{i=1}^d w_i x_i \right)$$

(python sample)
```
import numpy as np

np.sum(w, x)
```

- perceptron model hypotheses with bias/threshold w0

$$h(x) = sign \left( \sum_{i=1}^d w_i x_i + w0\right) = sign \left( \sum_{i=1}^d w_i x_i\right), (x_0=1)  = sign( W^T * X )$$

## git repo commands

### git repo setup and access

- setup ssh key
```
ssh-keygen -t rsa -b 4096 -C "<add-your-user-email-here>"
```

- after creating and accepting defaults, copy and paste id_rsa.pub contents to your github.com account ssh keys in admin
```
cat ~/.ssh/id_rsa.pub
```

- clone repo (crete first on github.com)
```
git clone git@github.com:<username>/educ-learning-from-data.git
```

- create a new repository on the command line
```
echo "# educ-learning-from-data" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:alanpmullane/educ-learning-from-data.git
git push -u origin main
```

-  push an existing repository from the command line
```
git remote add origin git@github.com:alanpmullane/educ-learning-from-data.git
git branch -M main
git push -u origin main
```

