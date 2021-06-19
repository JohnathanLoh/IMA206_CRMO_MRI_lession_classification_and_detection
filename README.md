# Détection de lésions dans des images IRM corps entier par réseaux de neurones

participants: Qingjie ZHANG, Jianshu ZHU, Johnathan Loh
Encadrants : Mateus Riva, Inès Mannes (radiologue), Isabelle Bloch

## Instructions for running the code

**For privacy reason, we don't put MRI images here**

### if you only want to test...
Open test.ipynb and modify the path (in the 4th cell) to the MRI image that you want to test, then run the whole program.

### if you want to train on your own dataset...
Open train.ipynb and modify carefully all the pathes needed with the help of the comments.

## Brief description of our model
### Classification 
In this section, we use CNN to extract features and SVM to classifiy the images in three categories: with lesion, without lesion, and uncertain.

### Detection
In this section, we propose the use of 2 different techniques. For both techniques, only images that have been identified/classified to have lesions in the previous section were used.

   1. Use of HOG to frame the regions with lesion. 

   2. Use of image thresholding to detect hyperintensities, followed by morphological opening to remove thin/line-like artifacts to create potential lesion region binary masks.

### Annotation
In this section, we use filter and morphology to annotate the possible lesions. Combined with the previous section, the lesions can be annotated and the artifacts can be eliminated. 


