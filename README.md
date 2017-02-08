# ds-ga-1008-a1

NYU course Spring 2017 Assignment 1

This sample code is modified from https://github.com/pytorch/examples/tree/master/mnist

60,000 training data was split into two parts. train_labeled.p contains 3000 labeled data and train_unlabeled.p contains 57000 data without labels. They are saved as torchvision.datasets objects.
 
Loading Data:

```python
import pickle
trainset_labeled = pickle.load(open("train_labeled.p", "rb"))
trainset_unlabeled = pickle.load(open("train_unlabeled.p", "rb"))
```

Training:
```bash
python mnist_pytorch.py
```
-Please go thourgh and understand the sample code.
 
-Apply techniques mentioned in section 2 to improve the performance in 3000 training data. We are more than happy to see that if you can implement other methods beyond section 2.

-Incoporate unlabeled data into this model. Try to implement some semi-supervised learning method.

Note: The sample code is tested on MacOS system, CPU, torch 0.1.7, Python 2.7.13 |Anaconda 4.3.0
