# Détection de lésions dans des images IRM corps entier par réseaux de neurones

participants: Qingjie ZHANG, Jianshu ZHU, Johnathan Loh
Encadrants : Mateus Riva, Inès Mannes (radiologue), Isabelle Bloch

## Classification 
In this section, we use CNN to extract features and SVM to classifiy the images in three categories: with lesion, without lesion, and uncertain.

## Detection
In this section, we use HOG to frame the regions with lesion. We only use the images classified with lesion in the previous section.

## Annotation
In this section, we use filter and morphology to annotate the possible lesions. Combined with the previous section, the lesions can be annotated and the artifacts can be eliminated. 


