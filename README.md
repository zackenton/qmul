# QMUL Machine Learning Session Setup Instructions

1. Get python 3.6
Recommended: https://www.anaconda.com/download/

The instructions which follow should be run in a terminal window (except the last command which should be entered in the jupyter notebook).

2. Build a conda environment (conda is a nice package manager for python). Run:
```
conda create --name qmul python=3.6 numpy matplotlib jupyter
```

3. Activate the environment
``` 
source activate qmul
```

4. Install tensorflow. The installation can be tricky, depending on your system. Easiest way is to use
```
conda install -c conda-forge tensorflow
```

5. Install keras
```
pip install keras
```

6. Check everything worked: first launch the jupyter notebook app:
```
jupyter notebook
```
this should open a browser window. Click the dropdown menu 'new' and select 'python 3'. This should open a new window which is a jupyter notebook - an interactive python playground. Check keras and its dependencies loaded by typing in the jupyter notebook (not in the terminal)
```
import keras
```
and hitting shift-enter. If it returns without an error, your installation worked!

(Note, in case people want to come back to this later, the versions used in the tutorial are tensorflow 1.4.0, keras 2.1.3)
