# Archimedes_Wind_Turbine
OpenFOAM case for the analysis of Archimedes wind Turbine

Archimedes wind turbine case using OpenFOAM.

Just follow these commands :- 

1.blockMesh

2.surfaceFeatureExtract

3.snappyHexMesh -overwrite

4.topoSet -dict system/createInletOutletSets.topoSetDict

5.createPatch -overwrite

6.decomposePar -force

7.foamJob -parallel -screen pimpleFoam


+ For SimpleFoam Case :- 


1.blockMesh

2.surfaceFeatureExtract

3.snappyHexMesh -overwrite

4.topoSet -dict system/createInletOutletSets.topoSetDict

5.createPatch -overwrite

6.decomposePar -force

7.foamJob -parallel -screen simpleFoam
