# CSE 455 Final Project — Model Accuracy Exploration with CIFAR-10

This repository contains the code and paper of the CSE455 Final project.

## group members

Jack Chuang, Warren Shen, Thomas Lin, John Cheng
University of Washington, March 2020

## Final Presentation Video

[Here is the link to the final presentation](https://youtu.be/7m5on6q3soQ)

## Github repository

[This is the link to the Github repository](https://github.com/Jack-Chuang/UW-CSE-455/tree/main/final%20project)

## Abstract

This project contains the training implementation with CIFAR-10 based on EfficientNet and Cutout. An integrational model is built with the idea of reinforced scaling and baseline. The best training result of the model is 87% accuracy.

- Implemented [NeRF](https://github.com/Jack-Chuang/CSE-490-G1/blob/49632543203b1f6369a5d04d41dfba719e90b655/final%20project/NeRF.pdf) and [D-NeRF](https://github.com/Jack-Chuang/CSE-490-G1/blob/49632543203b1f6369a5d04d41dfba719e90b655/final%20project/D-NeRF.pdf) using [Pytorch](https://pytorch.org/) based on their official Pytorch implementation.
- Recorded seven videos including two static scenes and five dynamic scenes.
- These videos were processed into training data.
- Then, trained different NeRF and D-NeRF models on different scenes.
  - D-NeRF: ≈ **200 hours**, ≈ **40 hours per scene**, 5 dynamic scenes, 400k iterations
  - NeRF: ≈ **175 hours**, ≈ **25 hours per scene**, 5 dynamic scenes, 2 static scenes, 400k iterations.
  - GPU: Nvidia Tesla P100
- Quantitatively and qualitatively, compared each novel view synthesis of each scene between its trained NeRF and D-NeRF models.

## Problem Description

This project looks at reproducing the implementation of NeRF and D-NeRF on static and dynamic scenes and comparing the two models on real-world data. One of the novelties of this project is performing the D-NeRF model on real-world scenes, where the original code from the author only deals with blender-type data(in virtual scenes). I am hoping to render a novel view synthesis of dynamic scenes of real-world objects by using D-NeRF and comparing it with the result of NeRF model on real-world data to prove that D-NeRF is indeed a real-world solution for dynamic scenes.
