# Global-Video-Copy-Detector
### By Benjamin Soto K.

## Detect copy between two videos using Global Characteristics (Ordinal Measurement Descriptor) of their images

## OpenGL Required (tested in version 3)
## Tested in python 3.6.5

## For the example, download the other videos (television) from https://drive.google.com/file/d/1PTmOOJiUPV34WixoT2kpKhYTYNYGZo2L/view?usp=sharing and put them in the television folder.

# Extract_Vid
### Extract global characteristics from videos in the folders "commercials" and "television", in order to do that, it uses the images of the video (one every 10 frames) then divides the images in a number of cells, calculating the mean grey intensity of each cell. While the width and height of the cells for each image can be different, the number of cells each row and column must be the same in every image. The result is saved in the folders "extract_tv" and "extract_com"
### In the example, television videos size are 768x432 and commercials 320x180.

# Copy_Detector
### Detect the images from the different videos that are close to each other, a threshold value is used to decide the max distance that copies candidates are selected. The result are in the folder "results" where each file is named after the video of the folder commercial in each file, first is the name of the video in the folder television that the commercial is compared to, and then are the images that a copy was detected, the format is "distance-minuteInTheCommercial-minuteInTheTelevision"

# Running the scripts
### 1 python Extract_Vid
### 2 python Copy_Detector

### In case of using different videos, be sure to check the proper call to the folders, extension of videos, the sizes of the cell and adjust the pace that images are taken (for example if you use a 60 fps video, either modify the rate that images are extracted, or change the way the minutes of a video are calculated when a copy is detected)
