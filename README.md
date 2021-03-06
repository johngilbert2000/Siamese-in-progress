# Siamese-in-progress
Siamese networks that almost work, written in Pytorch

<hr>

The files are as follows:

- `LFW_setup.ipynb`: run this to set up the LFW dataset for training. Originally this was stored in a folder labeled `/lfw`, which also contained the downloaded LFW dataset. (Directory setup example shown below).
- `APD_setup.ipynb`: run this to set up the APD dataset, if you have access to it. Note: originally the APD dataset was stored in a folder labeled `/data`, and the notebook `APD_setup.ipynb` was run in the directory containing the folder `/data` (i.e., one directory above the dataset APD)
- `siamese_LFW.ipynb`: run this in the directory above `/data` or `/lfw` to train a siamese network that doesn't yet work. I'm still unsure why. (Note: I recommend running each cell individually, so you know what each cell is doing, and in case the file paths are different).

Further descriptions are in the jupyter notebooks, along with further setup instructions.

Note: when you unzip the LFW dataset, it also creates a folder named `lfw`, so my directory structure was originally as follows:
```
├──`siamese_LFW.ipynb`
├──`APD_setup.ipynb`
├── `/data`
|    ├── `C.zip` (APD dataset)
|    └──`/C` (made from unzipping `C.zip`)
└──`/lfw`
     ├── `lfw.tgz`
     ├── `LFW_setup.ipynb`
     └──`/lfw` (made from unpacking `lfw.tgz`)
```

<hr>

To use the same Python environment that was originally used, download Anaconda (or Miniconda), then in the terminal, do the following:

```
    source anaconda3/bin/activate
    conda create -n fast2 python=3.7.7
    conda activate fast2
    conda install jupyter
    conda install -c conda-forge jupyter_contrib_nbextensions
    conda install -c pytorch -c fastai fastai pytorch torchvision cuda92
    conda install scikit-learn
    jupyter notebook
```
Note: I highly recommend using the `Collapsible Headings` and `Table of Contents (2)` jupyter notebook extensions

If you're new to jupyter notebooks, use `[shift]`+`[enter]` to run each selected cell individually.

For additional setup help, see:

https://github.com/johngilbert2000/code_shelf/blob/master/Jupyter_setup_tips.ipynb


