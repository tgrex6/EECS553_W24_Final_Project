# EECS553_W24_Final_Project
EECS 553 W24 Final Project, UMich, Ann Arbor

The major component of this project is basically a semantic segmentation task for the nucleus in H&E stained histology images of multi-organ tumor cells. Accurate segmentation of cell nuclei allows the analysis of key features like density, size ratios, and shape variations. These are critical for evaluating cancer severity and predicting treatment outcomes. In this project, we will employ UNet++ model to perform this task. UNet++ is a new general purpose image segmentation architecture for more accurate image segmentation. This architecture integrates a series of UNets with variable depths. These redesigned skip pathways are strategically devised to surmount two predominant limitations associated with the conventional UNet architecture: firstly, the indeterminate optimal depth, and secondly, the overly constricted configuration of skip connections.

## Dataset: [MoNuSeg 2018](https://monuseg.grand-challenge.org/Home/)[^1]
The dataset for this challenge was obtained by carefully annotating tissue images of several patients with tumors of different organs and who were diagnosed at multiple hospitals. This dataset was created by downloading H&E stained tissue images captured at 40x magnification from TCGA archive. H&E staining is a routine protocol to enhance the contrast of a tissue section and is commonly used for tumor assessment (grading, staging, etc.). Given the diversity of nuclei appearances across multiple organs and patients, and the richness of staining protocols adopted at multiple hospitals, the training datatset will enable the development of robust and generalizable nuclei segmentation techniques that will work right out of the box.
Official MATLAB Code for reading in xml annotations: [he_to_binary_masks_final.m](he_to_binary_mask_final.m)
Our Python version: he_to_binary_mask.py

[^1]: N. Kumar, R. Verma, S. Sharma, S. Bhargava, A. Vahadane and A. Sethi, "A Dataset and a Technique for Generalized Nuclear Segmentation for Computational Pathology," in IEEE Transactions on Medical Imaging, vol. 36, no. 7, pp. 1550-1560, July 2017, doi: 10.1109/TMI.2017.2677499. keywords: {Image segmentation;Measurement;Training;Machine learning;Image color analysis;Pathology;Diseases;Annotation;boundaries;dataset;deep learning;nuclear segmentation;nuclei},

