# Experiments
The MITgcm numerical experiment configurations utilized in the study by Aparco-Lara et al., 2023, are as follows:

![](https://img.shields.io/github/stars/JhonKevin3015/Experiments.svg) ![](https://img.shields.io/github/forks/JhonKevin3015/Experiments.svg) ![](https://img.shields.io/github/tag/JhonKevin3015/Experiments.svg) ![](https://img.shields.io/github/release/JhonKevin3015/Experiments.svg) ![](https://img.shields.io/github/issues/JhonKevin3015/Experiments.svg) 


##  EXP1 
Unforced case with KPP active
##	EXP2 
Forced case with KPP active
##	EXP3 
Unforced case with KPP inactive
##	EXP4 
Unforced case with KPP inactive
### General Description
* Each experiment folder contains a `code` and `input` subfolder. Within the `EXP*/CODE` folder, you will find two important files:
  - `packages.conf`: This file determines whether KPP is activated or deactivated for the specific experiment. It is set to activate KPP for EXP1 and EXP2 and deactivate KPP for EXP3 and EXP4.
  - `SIZE.h`: This file sets the number of processors used for the simulations.


* In `EXP*/input` folder, you can find the data files to modify the physical parameters, as well as the location where the Initial Conditions files obtained from Matlab codes in the `IC` folder should be placed.

* Additionally, in the `EXP2` and `EXP4` folders, you will find an additional file named `QnetIDE.forcing`, which contains the atmospheric forcing data.

* Each experiment folder contains outputs for the 15th day of simulation. This data was used to [generate figures](https://github.com/JhonKevin3015/VHFs) in Aparco-Lara et al., 2023.

  
### IC: Matlab-code to generate the initial conditions and Qnet-Forcing binary files.

* The binary obtained from `InitCondi.m` should be placed in each `EXP*/input/` folder.
* The `QnetIDE.forcing` obtained from `InitCondi.m` should be placed in the `EXP2/input/` and `EXP4/input/` folders.

For more information on how to run the simulations, refer to the [MITgcm tutorial (examples)](https://mitgcm.readthedocs.io/en/latest/examples/examples.html).
