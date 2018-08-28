# Global-Video-Copy-Detector
## Detect copy between two videos based with Global Characteristics (Ordinal Measurement Descriptor) using Python
## Videos are television 768x432 commercials 320x180

## OpenGL Required (tested in version 3)
## Tested in python 3.6.5

## For the example, download the other videos (television) from https://drive.google.com/file/d/1PTmOOJiUPV34WixoT2kpKhYTYNYGZo2L/view?usp=sharing and put them in the television folder.

# Extract_Vid
## Extract global characteristics from videos in the folders "commercials" and "television", in order to do that, it divides the image in a number of cells, calculating the mean grey intensity of each cell. While the width and height of the cells for each image can be different, the number of cells each row and column must be the same in every image.
In the example, television videos size are 768x432 and commercials 320x180.

# Copy_Detector

## 1 Run Extract_Vid
## 2 Run Copy_Detector
