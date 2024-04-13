# Archimedes_Wind_Turbine
OpenFOAM case for the analysis of Archimedes wind Turbine

![crab pet](https://imgur.com/a/uTa4jQM)

## Archimedes wind turbine case using OpenFOAM.

+ follow these commands:-
```
blockMesh

surfaceFeatureExtract

snappyHexMesh -overwrite

topoSet -dict system/createInletOutletSets.topoSetDict

createPatch -overwrite

decomposePar -force

foamJob -parallel -screen pimpleFoam
```

+ For SimpleFoam Case :-

```
blockMesh

surfaceFeatureExtract

snappyHexMesh -overwrite

topoSet -dict system/createInletOutletSets.topoSetDict

createPatch -overwrite

decomposePar -force

foamJob -parallel -screen simpleFoam
```
