# Pig Weight Estimation Pixel Occupancy Analysis
 The purpose of this research is to explore the possibility of new methods to estimate livestock weight based on pixel occupancy analysis. This study will focus on using a depth camera to obtain depth information for the target livestock, pigs, such as the number of pixels at each depth, and assigning different weights based on various depth information, to provide a weight estimate for the livestock. If the objectives of this study can be achieved, it can offer a novel approach to measuring livestock weight. Moreover, since the analysis focuses only on pixels, both the number and position of livestock can be disregarded, making the estimation of the weight of grouped livestock within a range possible. Theoretically, pixel occupancy analysis will utilize fewer resources for estimation, making it feasible to deploy on a single device and operate offline. If successful weight estimation is achieved on one type of livestock, this method could be applied to other types of livestock for weight estimation in the future. 

# Usage
### Install environment
All required dependencies are in 'requirements.txt', run these script to install the dependencies
```
pip install -r requirements.txt
```

### Data location
Please leave data images and weight in 'Data' Folder  

- Data/
  - Week1/
    - ...
    - ... (more files)
  - Week2/
    - ...
    - ...
  - final_mapping_original.csv
  - data.csv (use for training)

# File Distribution
- data_process.ipynb: Process raw image to pixel map.
- data_analysis_LR.ipynb: Linear regression model.
- data_analysis_XGBOOST.ipynb: XG Boost model.