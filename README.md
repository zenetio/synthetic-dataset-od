# Synthetic Dataset for Object Detection

## Introduction

This notebook is based on notebook of Alex P that can be found [here](https://github.com/alexppppp/synthetic-dataset-object-detection).

This project makes use of albumentatioos library to generate synthetic images. Albumentations is a fast and flexible image augmentation library project that can be found [here](https://github.com/albumentations-team/albumentations).

I've updated the notebook adding comments and the COCO format to the generated images.

In the figure below, the first image is the original image,

<p align="center">
    <img src="docs/original.jpg"  mode="center" width="800" height="400">
</p>

the second image is the augmented image and
<p align="center">
    <img src="docs/aug.jpg"  mode="center" width="800" height="400">
    <br></br>
</p>

 the third image is the augmented image with the bounding boxes.
<p align="center">
    <img src="docs/bbox.jpg"  mode="center" width="800" height="400">
    <br></br>
</p>

In the function `generate_dataset4coco()` you can define the number of augmented images you want to generate and the target operation: `train, valid, test`.<br>
The generator will provide the json file with bounding boxes for each image as well.

Enjoy!
