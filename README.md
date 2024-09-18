# Explicit-NeRF-QA：A Quality Assessment Database for Explicit NeRF Model Compression
## Introduction
In recent years, Neural Radiance Fields (NeRF) have demonstrated significant advantages in representing and synthesizing 3D scenes. Explicit NeRF models facilitate the practical NeRF applications with faster rendering speed, and also attract considerable attention in NeRF compression due to its huge storage cost. To address the challenge of the NeRF compression study, we construct a new dataset, called Explicit-NeRF-QA. 

We use 22 3D objects with diverse geometries, textures, and material complexities to train four typical explicit NeRF models across five parameter levels. Lossy compression is introduced during the model generation, pivoting the selection of key parameters such as hash table size for InstantNGP and voxel grid resolution for Plenoxels. By rendering NeRF samples to processed video sequences (PVS), a large scale subjective experiment with lab environment is conducted to collect subjective scores from 21 viewers. 

<img src=scenes.png width="400" alt="The source content in Explicit-NeRF-QA" align="center" />

## Dataset
The dataset include NeRF samples, source 3D objects, multiview images for NeRF generation, PVSs, MOS, is made publicly available at the following location: https://github.com/LittlericeChloe/Explicit-NeRF-QA.


