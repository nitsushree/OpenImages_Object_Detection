# OpenImages_Object_Detection

#### Requirements:
detecto custom installation (pip install detecto)

Problem Statement: To detect "Person" &amp; "Car" from the OpenImages dataset. 

### Dataset Details:

These images are taken from OpenImages
Link to download the dataset: https://evp-ml-data.s3.us-east-2.amazonaws.com/ml-interview/openimages-personcar/trainval.tar.gz

Number of images: 2239
Size: 750 MB (approx.)
Categories: 2 (person and car)
Annotation format: COCO

Custom_Detecto works on either Pascal VOC format or on CSV annotations. 
Convert COCO format to CSV (Code mentioned in the notebook)

#### Data directory structure:
data
|_ annotations
        |_ bbox-annotations.json
|_ images
        |_ image_000000001.jpg
        |_ image_000000002.jpg

#### Model: Custom Detecto Model
        . Architecture: FasterR-CNN_Resnet50_fpn
        . Optimizer: Can be choosen from torch module
        . Learning Rate: can be customised
        . Tensorboard integrated
        . GPU: configured
        
#### Inference:
Function calculates: IoU
Tensorboard activation to the directory to plot the events on localhost/jupyter notebook

