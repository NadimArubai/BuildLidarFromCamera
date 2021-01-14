# Building a Real-time 2D Lidar Using Deep Learning from a Camera

# Goal:
Building a real-time 2D Lidar by using a camera as an input, and by processing with deep learning.

# Reqiurment:
Python3.8 with:
Tensorflow 3.3
Keras 2.4.3
Matplotlib 3.1.2
opencv-python 4.5.1.48
python-gflags 3.1.2
scipy 1.6.0
scikit-learn 0.24.0

It should work if the versions is less or more than those, but it's tested with those versions.

# Dataset:
download Kitti from

https://www.hiast.edu.sy/sites/default/files/MasterPHD/5e6a1b73c2e7a.pdf

It needs the raw dataset and the annotated depth maps dataset.

Also the whole dataset is used {City, Person, Residintal, Road, Campus}.

After downloading the whole dataset, put it in one folder and use the script
```
python gen_triain_valid.py RAW_DATASET_FOLDER DEPTH_LABELS_FOLDER
```

to generate 2 folder: training and validation which contain the proper examples for training images and there depths labels.

# Training:
use:
```
python train.py
```

# Evalutaion:
```
python evaluate.py
```

# Testing
For testing on a small partition of the data set:

put any group of evaluation (or training) inside a Testing folder and run:
```
python test1.py
```

for a single view, while for showing the 3 layers use:
```
python test3.py
```

To measure time and frame rate use:
```
python mestime.py
```

# Doc
Here is the Master doc
https://www.hiast.edu.sy/sites/default/files/MasterPHD/5e6a1b73c2e7a.pdf

and here is the paper:
'to be added'

# TODO
- [ ] Cleaning the code from rubbish.

--- [ ] generate  [ ] test [ ] train.

- [ ] Adding proper commits.

--- [ ] generate  [ ] test [ ] train.

- [ ] Uploading

--- [ ] generate  [ ] test [ ] train.




