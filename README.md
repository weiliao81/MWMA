# MWMA
Multimodal, Multifaceted White Matter Atlas

Welcome to the MWMA package; a companion to our article "Multimodal, multifaceted imaging-based Human Brain White Matter Atlas".

# Software dependencies
MATLAB (tested on R2020a - https://www.mathworks.com/products/matlab.html)

# MWMA-50-400_atlas
The 50, 100, 150, 200, 250, 300, 350, 400-ROI MWMA and the white matter mask in nifti format are provided.

The functional network label file and the ITKSNAP-description file of the 200-ROI MWMA are provided.

# WM_parcellation_demo
The '01_code' file includes the subfunctions of parcellation procedure and the required tools packages.

The '02_data' file includes the example data from three subjects and the required files related to the White Matter mask.

There are four steps to generate the final group-level white matter atlas.

Step1: The inputs are the six imaging features (ALFF, dALFF, ReHo, DC, FA, MD in nifti format) for each subject, the output is the individual similarity matrix W in sparse form (in the 'sub_0X' folder).

Step2: The input is the individual similarity matrix W, the output is the individual level WM atlas with k ROIs in nifti format (in the 'sub_0X' folder).

Step3: The input is the individual WM atlas, the ouput is the group average adjacent matrix A_group (in the '02_data' folder).

Step4: The input is the group average adjacent matrix A_group, the output is the group-level atlas with k ROIs in nifti format (in the '02_data' folder).
