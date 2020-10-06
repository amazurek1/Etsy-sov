# To run images and outlines through model and run nearest neighbors for the images
everything_running_model_and_nearest_neighbors.ipynb

# SBIR regression
This repo contains code for the C&G paper "[Sketching out the details: Sketch-based image retrieval using convolutional neural networks with multi-stage regression](https://doi.org/10.1016/j.cag.2017.12.006)" 

## Dependencies
You will need to compile [Caffe v1.0](https://github.com/BVLC/caffe) with customized L2 normalize layer. Check [caffe_utils/README.md](caffe_utils/README.md) for instructions.

Alternatively, you can use standard Caffe, just remove the normalize layer in model/*.prototxt, then normalise the output manually using e.g. numpy.

## Pretrained model
Pretrained model (and dataset) can be downloaded [here](http://www.cvssp.org/data/Flickr25K/cag17.html).

## Feature extraction

Check [getfeat_img.py](getfeat_img.py) and [getfeat_skt.py](getfeat_skt.py) for examples of extracting features from a raw image/sketch.

## Demo
[![Youtube demo](http://img.youtube.com/vi/3FRDpNk4w4U/0.jpg)](https://youtu.be/3FRDpNk4w4U)

## Reference
```
@article{bui2018sketching,
  title={Sketching out the Details: Sketch-based Image Retrieval using Convolutional Neural Networks with Multi-stage Regression},
  author={Bui, Tu and Ribeiro, Leonardo and Ponti, Moacir and Collomosse, John},
  journal={Computers \& Graphics},
  year={2018},
  publisher={Elsevier}
}
```
