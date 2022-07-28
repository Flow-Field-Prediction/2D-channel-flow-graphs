# 2D-channel-flow-graphs

This is the data repository for the ICLR 2021 SimDL Workshop paper [DIRECT PREDICTION OF STEADY-STATE FLOW FIELDS IN MESHED DOMAIN WITH GRAPH NETWORKS](https://arxiv.org/pdf/2105.02575.pdf) by Lukas Harsch and Stefan Riedelbauch. If you like our work or want to use our data in your work, please cite this work by using

```
@misc{https://doi.org/10.48550/arxiv.2105.02575,
  author = {Harsch, Lukas and Riedelbauch, Stefan},
  title = {Direct Prediction of Steady-State Flow Fields in Meshed Domain with Graph Networks},
  publisher = {arXiv},
  year = {2021}
}
```

## Dataset

This reposit contains the data of 1300 CFD simulations of 2D channel flows, by solving the steady-state incompressible, inviscid Navier-Stokes equation. A varying number of generic objects is randomly placed inside the channel. Each simulation is represented by its `feature matrix` of shape Nx6, where N is the number of nodes. The node feature vector is given by: [x-position, y-position, velocity in x-direction, velocity in y-direction, preasure, node encoding (fluid, wall, object)]. Further, the node connectivities are given by the `connectivityDict`, where the current node is stated by the key and its neighboring nodes given by the dict values. The 1300 data samples are splitted into 4 folders.
