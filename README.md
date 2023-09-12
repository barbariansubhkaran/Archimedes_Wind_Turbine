# Archimedes_Wind_Turbine
OpenFOAM case for the analysis of Archimedes wind Turbine

## Archimedes wind turbine case using OpenFOAM.

Just follow these commands :-
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
