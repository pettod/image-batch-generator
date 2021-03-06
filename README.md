# Image Batch Generator

## Introduction

Image batch generator to work with image to image models. The generator returns batches of train and ground truth image pairs. The version 2 works with bursts as well.

## Installation and Data set Structure

The generator has been tested with Tensorflow versions 1.9.0 and 2.1.0 with Python 3.6. To use the generator only Tensorflow is needed to be installed. Version 2 does not use Tensorflow. To test the generator with given test script, install requirements below.

```bash
pip install -r requirements.txt
```

The train and ground truth data sets must have same file names and following folder structure:

```bash
data_folder/
    image_folder_1/
        image_1_1.png
        image_1_2.png
        image_1_3.png
        ...
        image_1_n.png
    image_folder_2/
        image_2_1.png
        image_2_2.png
        image_2_3.png
        ...
        image_2_n.png
    image_folder_3/
        image_3_1.png
        image_3_2.png
        image_3_3.png
        ...
        image_3_n.png
    .
    .
    .
    image_folder_m/
        image_m_1.png
        image_m_2.png
        image_m_3.png
        ...
        image_m_n.png
```

## Run Batch Visualization

1. Add data to the folders as described above.

1. Run `test_generator.py` to visualize batches. Add data sets as arguments in a following way:

```bash
python test_generator.py path/to/train_data path/to/ground_truth_data
```

**Note**: If ground truth data set path is not given, batches will only be shown for train data set.
