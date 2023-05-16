# ISRO_Chandrayan_Moon_Mapping
Chandrayaan moon mapping problem was proposed by the ISRO (Indian Space Research Organization) in the Inter IIT tech meet 11.0 held at IIT Kanpur.  Our team (Sourav Saini, Aashray Gupta, Aayush Gupta, Divyansh Mundra, Falak Singla, Sanath Naveen Sharma, Satyansh Sharma) from IIT Jammu, won Silver Medal.

## Introduction

The Chandrayaan-2 Mission of ISRO was launched on July 22, 2019 from the Indian Space Port, Sriharikota by GSLV Mk-III. It was a highly complex mission comprising many new technological developments. The mission is designed to expand the lunar scientific knowledge through detailed study of topography, mineral identification and distribution, surface chemical composition, as well as the lunar exosphere. 

The Chandrayaan-2 Orbiter carry total eight scientific payloads. The Orbiter Higher Resolution Camera (OHRC) onboard Chadrayaan-2 Orbiter is an imaging payloads which provides high resolution (~ 30 cm) images of lunar surface. The Terrain Mapping Camera-2 (TMC-2) Chadrayaan-2 Orbiter maps the lunar surface in the panchromatic spectral band (0.5-0.8 microns) with a spatial resolution of 5 meter. The data collected by TMC-2 provides clues about the Moon’s evolution and help prepare 3D maps of the lunar surface.

The problem statement is divided in two parts:

Part 1

Development of an AI/ML model to generate high (~30 cm) resolution lunar terrain image from medium/low (5 m / 10 m) resolution terrain image, and evaluate its accuracy; the model will be amenable to further training and improvement.


Part 2

To generate a global lunar atlas (digital) with the help of the AI/ML model, based on the medium / low resolution data available. The AI/ML model to be developed by using the publically available overlapping data of OHRC (~30 cm resolution) and TMC-2 (5 m /10 m resolution) payload data on board Chandrayaan-2 Orbiter.

## How to use our custom model:

**Caution** : Please run the google colab notebook on gpu.

Create a shortcut of Real-ESRGAN-master:
Go to the link [Real-ESRGAN-master](https://drive.google.com/drive/folders/1MMRjSXpHObHC2czmbljown8ILGOTrXpl), right click on Real-ESRGAN-master folder, and select the option add a shortcut to drive, then click on add shortcut.

Execute the colab notebook as mentioned in the notebook, block by block.

Please put the path of the input image in the “image_input_path” variable in the last block of code.
Also, put the path of the output image in the  “image_output_path” variable in the last block of code.
image_input_path = "sample_input.png"
image_output_path = "sample_output.png"
Super_res(image_input_path , image_output_path)

Note : Our final model is present in custom_model.
Software Requirements :  If you are running the model on normal version of colab, then GPU RAM will overflow. So, please use small sized images to model, or slice the image in small parts.

Citations:  
Cite as:
arXiv:2107.10833 [eess.IV]
 
(or arXiv:2107.10833v2 [eess.IV] for this version)
 
https://doi.org/10.48550/arXiv.2107.10833


References:
Real-ESRGAN: Training Real-World Blind Super-Resolution with Pure Synthetic Data
Xintao Wang, Liangbin Xie, Chao Dong, Ying Shan
