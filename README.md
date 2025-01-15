# Deep-Learning-Based-Conjunctival-Melanoma-Detection

**References of research papers used:**
1. Adopting low-shot deep learning for the detection of conjunctival melanoma using ocular surface images: (Tae Keun Yoo, et al. - 2023)


2. Deep Learning-Based Conjunctival Melanoma Detection Using Ocular Surface Images: (Kanchon Kanti Podder et al. - 2021)


**Dataset source: ** http://dx.doi.org/10.17632/t75wjsw6bw  (images were verified by ophthalmologists) 

Input dataset: Eye images (Ocular Surface Images)



This is a project implemented as part of Semester 8, for the Deep Learning Elective course (during my Integrated MTech course).



Four main categories of images in dataset: Normal Conjunctiva (96 images), Pterygium (75 images), Nevus (86 images) and Conjunctival Melanoma (139 images)

Due to the small size of dataset, 4 different data augmentation techniques were applied to increase the number of images in the different classes:

Random rotation                              (+20 to -20 degree range)

Random affine transformation      (degree = 0, translate range = (0.05, 0.15), scaling range = (0.9, 0.95))

Padding                                               (range = (0, 10), fill = (black, white), mode = (constant, edge))

Color correction                                (brightness = (0, 0.2), contrast = (0, 0.2)) 



GAN techniques were used for data augmentation:  Considering dataset with 2-classes “normal” and “abnormal” containing 4000 images each, a PyTorch-based GAN Model is considered.
Image Classification was also performed with PyTorch-based CNN models, Transfer Learning with MobileNetv2 Model, and EfficientNetB7 Model.
The Grad-CAM technique was also explored.


Group members:
S. Anusri (20MCME31)
M. Bhagya Sree (20MCME01)
Ankith Mall (20MCME19) and
G. Srinivas (20MCME06)



