# Archimedes_Wind_Turbine
OpenFOAM case for the analysis of Archimedes wind Turbine

<img src="https://d2t1xqejof9utc.cloudfront.net/screenshots/pics/59a67a0f22cab77943c1abeb7c5fcd26/large.png" />

## Archimedes wind turbine case using OpenFOAM.

+ Just follow these commands :-
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
