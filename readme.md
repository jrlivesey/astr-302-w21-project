# protoplanet

```protoplanet``` is a simple Python code for quickly making new ```VPLanet``` input directories from pre-existing ones. Run ```protoplanet``` from a path containing a directory with your input files for a given simulation. A new directory with your specified changes will appear in a new directory. Note that only ```.in``` files will be copied/modified. The new simulation you've created can then be run in the usual way, by navigating to this new directory and using the command:

```
vplanet vpl.in
```

To clone ```VPLanet``` and for more information please see the [VPLanet GitHub page](https://github.com/VirtualPlanetaryLaboratory/vplanet).

## Expected usage
Suppose you want to copy a ```VPLanet``` simulation, hosted in a directory called ```dir```, with modifications to two files, ```b.in``` and ```c.in```. You want to set the inclination angle of planet b to 90 degrees, and set the orbital eccentricity of planet c to 0.1. To do this, the appropriate command with ```protoplanet``` would be:

```
./protoplanet -d dir -p b:dInc=90 c:dEcc=0.1
```

One may alter as many parameters as they want using ```protoplanet```, but beyond a certain point it might actually be quicker to manually copy the directory and alter the input files.
