# CPIA_data_process

The CPIA dataset contains 3,474,406 (the total number is growing as we continue to process the datasets) standardized images, covering over 50 organs/tissues and about 98 kinds of diseases, which includes two main data types: whole slide images (WSIs) and characteristic regions of interest (ROIs).

In this repo, we provide relevant codes for processing all sub-datasets within the CPIA dataset. 

![image](https://github.com/Desperadodo/CPIA_data_process/assets/87553719/ec9631e0-c398-4711-9eca-b764333ef10b)
*The compositions and WSI processing strategy of the CPIA dataset.*

![image](https://github.com/Desperadodo/CPIA_data_process/assets/87553719/2f8660a5-429d-4e42-97f5-8bc5eeb4c587)
*The multi-scale strategy and diverse characteristics of the CPIA dataset.*

## WSI
Each WSI dataset is divided into four levels using one python program. Most of the Whole Slide Imaging (WSI) images are stored in the SVS format, which includes the micron-per-pixel (MPP) information in the header file. Our processing program can automatically identify the MPP of each image and standardize it to 0.4942um/pixel by adjusting the edge length of each patch. Finally, the patch images are divided into four different sizes with edge lengths of 3840, 960, 384, and 96, respectively, and stored in their respective folders.

|CAM16|
|CATCH dataset|
|CMB-CRC|
|CMB-LCA|
CMB-MEL
CPTAC-AML
CPTAC-BRCA
CPTAC-CCRCC
CPTAC-CM
CPTAC-COAD
CPTAC-HNSCC
CPTAC-LSCC
CPTAC-LUAD
CPTAC-OV
CPTAC-PDA
CPTAC-SAR
CPTAC-UCEC
HER2 tumor ROIs
MSKCC(SLN-Breast)
PAIP2019
PAIP2020
PAIP2021
Post-NAT-BRCA
TCGA-ACC
TCGA-BLCA
TCGA-BRCA
TCGA-CESC
TCGA-CHOL
TCGA-COAD
TCGA-DLBC
TCGA-ESCA
TCGA-GBM
TCGA-HNSC
TCGA-KICH
TCGA-KIRC
TCGA-KIRP
TCGA-LGG
TCGA-LIHC
TCGA-LUAD
TCGA-LUSC
TCGA-MESO
TCGA-OV
TCGA-PAAD
TCGA-PCPG
TCGA-PRAD
TCGA-READ
TCGA-SARC
TCGA-SKCM
TCGA-STAD
TCGA-TGCT
TCGA-THCA
TCGA-THYM
TCGA-UCEC
TCGA-UCS
TCGA-UVM





The processing code for the ROI dataset is related to the structure of the original dataset. After the processing is complete, each dataset folder contains only all images of that dataset, with each image having a dimension of 384x384 pixels, and is stored in jpg format. 

Before processing the data, please ensure that only the target images to be processed are contained in the input path of the program, and enter the correct suffix of the images to be processed (this might require slight adjustments to the original dataset folder).
  
![image](https://github.com/Desperadodo/CPIA_data_process/assets/87553719/6a97801d-c104-4224-8458-5c5ffeafb738)


