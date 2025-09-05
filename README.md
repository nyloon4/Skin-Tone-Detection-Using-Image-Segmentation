# Skin-Tone-Detection-Using-Image-Segmentation

## Overview
This project applies image segmentation techniques to detect skin-tone regions in facial images.  
The workflow reduces raw image data into principal components and uses distance thresholds to identify regions most likely representing skin tones.

## Methods
- Converted images from **BGR to RGB** format for accurate color representation.  
- Masked the dataset to remove non-skin values and isolate relevant color ranges.  
- Constructed **Gram matrices** and calculated eigenvalues/vectors.  
- Applied **Principal Component Analysis (PCA)** to reduce dimensionality by ~60% while preserving key variance.  
- Classified pixels within a distance threshold of the first PCA axis as skin tones.  

## Results
- Accurately identified skin-tone regions in facial images.  
- Achieved **~95% accuracy** in segmentation performance.  
- Produced visual outputs confirming alignment with known skin-tone distributions.  

## Tools Used
- Python  
- NumPy, pandas, Matplotlib  
- OpenCV  
- scikit-learn (PCA)  

## Repo Structure
- **`notebooks/`** → Jupyter notebooks for analysis and experimentation 
- **`figures/`** → Saved outputs such as graphs and example segmentations  
