## Example

The directory ```initial``` contains the input files for one of the sample simulations included on the ```VPLanet``` documentation ([here](https://github.com/VirtualPlanetaryLaboratory/vplanet/tree/master/examples/CassiniMulti)). The two planets involved are Teegarden's Star b and c. Suppose you were playing with this simulation and wanted to run one of your own. You are curious as to how the results would be altered if TG b were, in fact, a watery world (translating to a tidal quality factor of closer to Earth's value of 12 than the original 100) with an obliquity of 45 degrees. Further, you are curious what would transpire in the event that TG c has a perfectly circular orbit (eccentricity of zero). You can quickly find out by using the ```protoplanet``` command

```
./protoplanet -d initial -p TGb:dObliquity=45.0 TGb:dTidalQ=12 TGc:dEcc=0.0
```

and running ```VPLanet``` using the new input files this produces. The result in this case is shown in the directory ```final```. Note that the initial directory contains another, non-input file, namely a PDF figure, and this is not transferred to the final directory.
