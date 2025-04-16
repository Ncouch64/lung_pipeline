# Pulmonary Nodule Detection and Classification in Lung CT

# Primary approach
Two stages
- First the full detection and classification pipeline
- Second the model optimization steps to see how much the model can be reduced to work on low compute devices while still showing decent results.

Summary
• Develop a deep learning model to detect and classify pulmonary nodules (benign
vs. malignant) in 3D lung CT scans.
• Focus on building an automated pipeline that includes both nodule localization
and classification.
• Evaluate performance using sensitivity, specificity, and detection F1 scores.
Why It’s Interesting
• Early detection of malignant nodules is crucial for improving lung cancer survival
rates.
• Offers the chance to explore 2D vs. 3D CNNs or advanced transformer-based
architectures for volumetric data.
Dataset
• LIDC-IDRI Dataset (Lung Image Database Consortium and Image Database
Resource Initiative)
• Link: https://wiki.cancerimagingarchive.net/display/Public/LIDC-IDRI
Potential Approaches
• 3D CNN-based Detection: Use networks such as 3D U-Net or VNet to segment
and locate nodules.
• Classification Module: Use a secondary CNN or transformer to classify nodule
patches as benign or malignant.
• Multi-task Learning: Combine detection and classification in one framework for
efficiency.
References/Resources
1. Data Source (LIDC-IDRI):
https://wiki.cancerimagingarchive.net/display/Public/LIDC-IDRI
2. 3D U-Net Paper: Çiçek, Ö., Abdulkadir, A., Lienkamp, S.S., et al. “3D U-Net:
Learning Dense Volumetric Segmentation from Sparse Annotation.” MICCAI, 2016.
3. Transformer for 3D: Hatamizadeh, A., et al. “UNETR: Transformers for 3D
Medical Image Segmentation.” arXiv preprint, 2021

# Basic structure of pres
1. Problem
2. Related Work
3. Dataset
4. Methodology
5. Results so Far
6. Future Work

Interested in doing a quantization and optimization pass to see if I can get the model running quickly. This could be one aspect of the project.
In addition, depening on the dataset a novel pass at augmentation maybe. Might be too rough though as I think labeling would be required.