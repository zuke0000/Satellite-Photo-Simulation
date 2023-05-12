# Satellite-Photo-Simulation
A research project in Blender.

[Here is a report]([url](https://docs.google.com/document/d/1F1ux6iJLPZb3-dmgNmj_rlfazX_pNTuOhnVxNCUzOFY/edit?usp=sharing)) on this repository, using it in a model to test the the impact.

Here is a [tutorial](https://docs.google.com/document/d/1d491qWyg2AbIjXmX4eZGi1FXa6G3qNfWa6E2ae9TwUs/edit?usp=sharing) on how to create this project from scratch. The tutorial is a simulation of Chicago-9 from the [Inria dataset](https://project.inria.fr/aerialimagelabeling/)

A picture of the simulation and groundtruth were plugged in to a model using various scripts from [Models for Remote Sensing](https://github.com/bohaohuang/mrs). The encoder used is Resnet34 and the decoder is UNet. Due to time constraints the model was only trained up to 10 epochs.

## Results
| Training Data      | Validation Score (IoU) at 10 Epochs |
| ----------- | ----------- |
| Inria (No Chicago)     | 0.686     |
| Inria (With Chicago Simulation)   |     0.712    |
| Inria (With Chicago Simulation and Real)   | 0.679  |
- More results can be seen from the graphs seen in the [report]([url](https://docs.google.com/document/d/1F1ux6iJLPZb3-dmgNmj_rlfazX_pNTuOhnVxNCUzOFY/edit?usp=sharing)) and the evaluation notebook. TODO
- As mentioned in the report the results are not indicitive that the simulation actually improves the model due to the low epoch count.

## Improvements to be made
- Trees should not collide with buildings
- Shadows can look more realistic
- Building colors are too saturated with color
- Geometry nodes is a possible avenue of procedurally generating areas
