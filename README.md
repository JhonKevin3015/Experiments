# Experiments
The MITgcm numerical experiment configurations utilized in the study by Aparco-Lara et al., 2023, are as follows:

##  EXP1 
Unforced case with KPP active
##	EXP2 
Forced case with KPP active
##	EXP3 
Unforced case with KPP inactive
##	EXP4 
Unforced case with KPP inactive
### General Description
Each experiment folder contains a code package and input files. The `EXP*\CODE` folder includes two important files: `packages.conf`, where KPP is turned on for `EXP1` and `EXP2`, and turned off for `EXP3` and `EXP4`; and the file `SIZE.h` which is set to use 25 processors.

The `input` folder contains binary files for initial conditions, where `EXP2` and `EXP4` have `QnetIDE.forcing` files for atmospheric forcing
The data file includes all physical parameters.

## IC: Matlab-code to generate the binaries files of the initial conditions and Qnet-Forcing.

The binary obtened from `InitCondi.m` should be placed in:  `EXP*/input/` .
The `QnetIDE.forcing` obtened from `InitCondi.m` should be placed in the:  `EXP2/input/` , and `EXP4/input/`

For more information on how to run the simulations and a detailed tutorial on using the MITgcm ocean model, please refer to the following link: 
[Mitgcm:Examples](https://mitgcm.readthedocs.io/en/latest/examples/examples.html).
