# Facial Landmark Detection using PIPNet

## Description

This project implements facial landmark detection using the PIPNet model from the torchlm library.

PIPNet is trained to detect landmarks on facial images by predicting heatmaps for key points like eyes, nose, mouth etc. 

The model is trained and evaluated on a dataset of over 700 facial images collected at Shahid Beheshti University.

## Model

PIPNet (A Pixel-wise Implicit Representation based Network) from [torchlm](https://github.com/tritechpte/torchlm) is used. 

It is an efficient model that predicts pixel-wise heatmaps for landmarks.

## Training Data

- Facial image dataset with over 700 samples
- Collected at Shahid Beheshti University
- Variety of illumination, poses, expressions etc.

## Training Process 

- PIPNet is initialized with pretrained weights
- Fine-tuned on the facial image dataset 
- Optimized using Adam optimizer
- Trained for multiple epochs with learning rate decay

## Evaluation

The model is evaluated on test data using landmark detection metrics:

- Normalized Mean Error (NME)
- Failure Rate for different thresholds

## Usage

The trained PIPNet model can be used for:

- Detecting facial landmarks in new images
- Processing faces for tasks like alignment

## References

- [PIPNet Paper](https://arxiv.org/pdf/2003.03771.pdf)
- [torchlm Library](https://github.com/deftruth/torchlm)
