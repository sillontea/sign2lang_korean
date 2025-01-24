# Data Construction
## 1. Install Libraries
```bash
# opencv with conda
conda install -c conda-forge opencv
# opencv with pip
pip install opencv

# install uuid
pip install uuid
```
## 2. Capture Images
Capture 10 images per class.
Open the class file, keep only the classes you want to label, and delete the rest.
Run CaptureVideo.ipynb.
Execute the cells in order.
Verify that the files are saved correctly before proceeding to the next step.

## 3. Create Labels (VOC Format)
To create labels, run ybat.html:
```bash
$ annotation_tools/ybat-master/ybat.html
```
- Use the VOC dataset format for labeling.
- The VOC format saves data as XML files.

1. Load the images:
- Image save path: ```images/{class}```
2. Load the class information file:
- Class file path: ```./class.txt```
3. Select the corresponding class in Classes and draw a box at the appropriate location on the right-hand side of the image screen.
4. Use Save VOC (bottom-right) to save the file containing the class information.
