# Satellite-Photo-Simulation
A research project in Blender. 

Here is a [tutorial](https://docs.google.com/document/d/1d491qWyg2AbIjXmX4eZGi1FXa6G3qNfWa6E2ae9TwUs/edit?usp=sharing) on how to create this project from scratch. The tutorial is a simulation of Chicago-9 from the [Inria dataset](https://project.inria.fr/aerialimagelabeling/)

A picture of the simulation and groundtruth were plugged in to a model using various scripts from [Models for Remote Sensing](https://github.com/bohaohuang/mrs). The encoder used is Resnet34 and the decoder is UNet.

## Results
| Training Data      | Score (IoU) |
| ----------- | ----------- |
| Inria (No Chicago)     | TBA     |
| Inria (With Chicago Simulation)   | TBA        |
| Inria (With Chicago Simulation and Real)   | TBA        |

## Improvements to be made
- Trees should not collide with buildings
- Shadows can look more realistic
- Building colors are too saturated with color
- Geometry nodes is a possible avenue of procedurally generating areas
