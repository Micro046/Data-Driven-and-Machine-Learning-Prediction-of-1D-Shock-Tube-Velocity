# Data-Driven Prediction of 1D Shock-Tube Velocity

This repository contains the pressure and velocity data used for a small project on predicting the behavior of a 1D compressible gas flow in a shock tube.

The main idea of the project is simple:

- use pressure data `p(x,t)` as the input
- predict velocity data `u(x,t)` as the output
- compare data-driven and machine-learning methods

The data files are:

- `project/pressure.txt`
- `project/velocity.txt`

In both files, the first column is the spatial coordinate `x`. The remaining columns are time snapshots of the field.

So each row represents one spatial location, and each column after the first one represents the value at a different time.

The project compares methods such as DMD, DMD with control, SINDYc, Ridge regression, MLP, and LSTM. The results are evaluated using prediction error and training time.
