# BdPy

[![PyPI version](https://badge.fury.io/py/bdpy.svg)](https://badge.fury.io/py/bdpy)
[![GitHub license](https://img.shields.io/github/license/KamitaniLab/bdpy)](https://github.com/KamitaniLab/bdpy/blob/master/LICENSE)

Python package for brain decoding analysis

## Requirements

- Python 2.7, 3.6, or later
- numpy
- scipy
- scikit-learn
- h5py

### Optional requirements

- `dataform` module
    - hdf5storage
    - pandas
- `dl.caffe` module
    - Caffe
    - PIL
    - tqdm
- `dl.torch` module
    - PyTorch
    - PIL
- `fig` module
    - matplotlib
    - PIL
- `mri` module
    - nipy
    - nibabel
    - pandas

## Installation

``` shell
$ pip install bdpy
```

## Packages

- bdata: BdPy data format (BData) core package
- dataform: Utilities for various data format
- distcomp: Distributed computation utilities
- dl: Deep learning utilities
- feature: Utilities for DNN features
- fig: Utilities for figure creation
- ml: Machine learning utilities
- mri: MRI utilities
- opendata: Open data utilities
- preproc: Utilities for preprocessing
- stats: Utilities for statistics
- util: Miscellaneous utilities

## BdPy data format

BdPy data format (or BrainDecoderToolbox2 data format; BData) consists of two variables: dataset and metadata. **dataset** stores brain activity data (e.g., voxel signal value for fMRI data), target variables (e.g., ID of stimuli for vision experiments), and additional information specifying experimental design (e.g., run and block numbers for fMRI experiments). Each row corresponds to a single 'sample', and each column representes either single feature (voxel), target, or experiment design information. **metadata** contains data describing meta-information for each column in dataset.

See [BData API examples](https://github.com/KamitaniLab/bdpy/blob/master/docs/bdata_api_examples.md) for useage of BData.

## Developers

- Shuntaro C. Aoki (Kyoto Univ)
