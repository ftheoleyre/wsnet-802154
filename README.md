![](https://img.shields.io/badge/C-00599C-green)
![](https://img.shields.io/badge/Shell_Script)


This repository provides an implementation of the beacon-enabled mode of IEEE 802.15.4-2006. More precisely, it implements the main following features:

- synchronization with beacons
- one superframe per coordinator
- sleeping mode between two superframes
- only the upward direction is implemented

# Installation

You can first take a look at the documentation of the wsnet simulator : wsnet.gforge.inria.fr/.
Some parts of the simulator have been modified, and you need to copy the corresponding file in the main simulator directory.

The installation is described separately in the INSTALL file.  

# Execution

You can generate a sequence of simulations, to measure the impact of:
* number of nodes
* number of parents
* broadcast algorithm
* BO/SO values

More precisely, each script generates batches of jobs (one job = one siumulation with a set of parameters). Then, you can choose to execute all these jobs:
* standalone: a single computer executes everything
* hpc: a high performance computing infrastructure executes all the jobs on a large set of computing nodes (with torque to describe each job)
