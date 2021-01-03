## README

### copyright

- this repository is jupyter-version of [Li-Chongyi](https://github.com/Li-Chongyi)/**[Zero-DCE](https://github.com/Li-Chongyi/Zero-DCE)**
- ONLY NON-COMMERCIAL USE is APPROVED

### file structure

```bash
├─data
│  ├─test_data
│  │  ├─DICM
│  │  └─LIME
│  └─train_data
└─snapshots
```

### dataset prepare

tips can be checked in [here](https://github.com/Li-Chongyi/Zero-DCE#train)

### colab users

- for gpu users, click [here](https://colab.research.google.com/drive/1Blnsb4KQaI_voyxJYXRHT2sUxIJzsrH_?usp=sharing)
- for cpu users, click [here](https://colab.research.google.com/drive/1dkBrs1s9fHNKA3HfmhLSxHIrMJVpv4qm?usp=sharing)

### experimental facility

- if gpu available, please uncomment "for gpu users" statement and comment "for cpu users" statement
- if not, no need to modify anything

### python environment setting

- python 3.7
- torch - pip install torch
- torchvision - pip install torchvision

### experimental parameters setting, tips is highlighted by code comment

- paths
    - training data path - default is 'L:\\teng\\Documents\\zdce\\data\\train_data\\', edit in the 2nd cell in Sec.data_loader
- optimizer
    - weight decay - default is 0.0001, edit in the 3rd cell in Sec.data_loader
    - learning rate - default is 0.0001, edit in the 1st cell in Sec.training_function
    - grad_clip_norm - default is 0.1, edit in the first cell in Sec.training_function
- training
    - epochs - default is 200, edit in the first cell in Sec.training_function
    - batch_size - default is 1, edit in the first cell in Sec.training_function
    - num_workers(mul-processings) - default is 0, edit in the first cell in Sec.training_function
    - display training iters - default is 50, edit in the first cell in Sec.training_function
    - save checkpoint iters - default is 100, edit in the first cell in Sec.training_function
    - checkpoint save folder path - default is "snapshots/", edit in the first cell in Sec.training_function

### moreover

if meet issues, please put forward issues in [board](https://github.com/litun5315/zdce/issues) or mail me
