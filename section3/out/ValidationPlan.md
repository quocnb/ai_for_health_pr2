
## Validation Plan

### 1. General Information:

**Intended Use:**  
Integrated into a clinical network to assist a radiologist with quantifying Hippocampus volume for Alzheimer’s progression.

**Indications for Use:**  
It can be used for both male and female patients using MRI images.

**Limitations:**  
- This AI algorithm will perform well when the input data is cut to a rectangular portion of a brain scan rom every image series for a volume in the NIFTI format.
- Require high-power processing computer to run the algorithm


### 2. Dataset 

We are using the "Hippocampus" dataset from the Medical Decathlon competition.   
This dataset is stored as a collection of NIFTI files, with one file per volume, and one file per corresponding segmentation mask.   


### 3. Algorithm Performance
**Metrics**  
Two metrics are used to measure the performance of the algorithm: 
- Jaccard Similarity Coefficient
- Dice Similarity Coefficient 

**Performance on given dataset**  
The algorithm can achieve a Dice Similarity Coefficient approximately 0.90 and Jaccard Similarity Coefficient approximately 0.82

### 4. Real-world Inference
- The algorithm can only perform on T2 MRI brain scan.
- The algorithm cannot perform on other image format such as CT scan. 
- The algorithm can only be used to measure volume of hippocampus of the brain. 