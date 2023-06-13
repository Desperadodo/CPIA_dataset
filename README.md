# CPIA_data_process\

The CPIA dataset contains 3,474,406 (the total number is growing as we continue to process the datasets) standardized images, covering over 50 organs/tissues and about 98 kinds of diseases, which includes two main data types: whole slide images (WSIs) and characteristic regions of interest (ROIs).

In this repo, we provide relevant codes for processing all sub-datasets within the CPIA dataset. 

![image](https://github.com/Desperadodo/CPIA_data_process/assets/87553719/ec9631e0-c398-4711-9eca-b764333ef10b)
*The compositions and WSI processing strategy of the CPIA dataset.*

![image](https://github.com/Desperadodo/CPIA_data_process/assets/87553719/2f8660a5-429d-4e42-97f5-8bc5eeb4c587)



The WSI dataset is divided into four levels using the same program. The processing code for the ROI dataset is related to the structure of the original dataset. After the processing is complete, each dataset folder contains only all images of that dataset, with each image having a dimension of 384x384 pixels, and is stored in jpg format. 

Before processing the data, please ensure that only the target images to be processed are contained in the input path of the program, and enter the correct suffix of the images to be processed (this might require slight adjustments to the original dataset folder).
  
![image](https://github.com/Desperadodo/CPIA_data_process/assets/87553719/6a97801d-c104-4224-8458-5c5ffeafb738)


