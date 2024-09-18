# Explicit-NeRF-QA：A Quality Assessment Database for Explicit NeRF Model Compression
## Introduction
In recent years, Neural Radiance Fields (NeRF) have demonstrated significant advantages in representing and synthesizing 3D scenes. Explicit NeRF models facilitate the practical NeRF applications with faster rendering speed, and also attract considerable attention in NeRF compression due to its huge storage cost. To address the challenge of the NeRF compression study, we construct a new dataset, called Explicit-NeRF-QA. 

We use 22 3D objects with diverse geometries, textures, and material complexities to train four typical explicit NeRF models across five parameter levels. Lossy compression is introduced during the model generation, pivoting the selection of key parameters such as hash table size for InstantNGP and voxel grid resolution for Plenoxels. By rendering NeRF samples to processed video sequences (PVS), a large scale subjective experiment with lab environment is conducted to collect subjective scores from 21 viewers. 
<p align="center">
 <img src=scenes.png width="500" alt="The source content in Explicit-NeRF-QA" align="center" >
</p>

## Dataset
The dataset include NeRF samples, source 3D objects, multiview images for NeRF generation, PVSs, MOS, is made publicly available at the following location: https://github.com/LittlericeChloe/Explicit-NeRF-QA.

The dataset includes: 

(1) "Multiview images & Camera files" folder: 

It contains multiview images along with corresponding '.json' camera parameter files for 22 3D models which consist of three parts: training (train) , testing(test) and validation(val) set. The training set act as input for training NeRF models, testing set is used to calculate objective metrics, and validation set is used to render videos for subjective experiments.

(2) "NeRFs" folder:

It contains all the 440 NeRF model files used in our project. Specifically, we use 22 synthetic 3D scenes and 4 explicit NeRF models each with 5 quality levels corresponding to different compression levels, resulting in a total of 440 NeRF model files.

(3) "Videos" folder:

It contains all the 440 videos used in the subjective experiment. 

(4) "MOS.xlxs":

420 MOS scores obtained form subjective experiment are listed. (another 20 samples are used in training sessions in subjective experiment)

(5) "Datasource.txt": 

Source location of all the 3D models are listed.


