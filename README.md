Panoramic Image Stitching
Create panorama image from given set of overlapping images.

Requirements
numpy >= 1.24.3
opencv-python >= 4.9.0 (latest as of 2024)
opencv-contrib-python >= 4.9.0 (latest as of 2024)
imutils >= 0.5.4
Description
We have implemented the panoramic image stitching algorithm using invariant features from scratch. We have Implemented the David Lowe research paper on "Panoramic Image Stitching using Invariant Features". Used SIFT to detect features, RANSAC, Homography and Warp Prespective concepts.

About Data
NOTE: You can experiment with any images (of your own choice). We have experimented with many which you can find in data/ folder. Please check the results below.

Sample Images
Repo already provides sample images present in data/ folder. Copy images from data/ folder and put it into inputs/ folder.
Default: you will find data/tajm folder images in inputs/ folder.
Custom Images
You can create your own images as well and put it into inputs/ folder.

Make sure your images must be in sequence and have overlapping parts between consecutive images.
Minimum width and height for all images should be 400.
How To Run
Put images in inputs/ folder from which you want to create panorama image.
Run:
python3 stitch.py
Enter the number of images you want to concatenate (i.e number of images present in inputs/ folder):
Enter the number of images you want to concatenate: 4
Keep entering the images name along with path and extension. For Ex:
Enter the image names with extension in order of left to right in the way you want to concatenate: 
Enter the 1 image name along with path and extension: inputs/tajm1.jpg
Enter the 2 image name along with path and extension: inputs/tajm2.jpg
Enter the 3 image name along with path and extension: inputs/tajm3.jpg
Enter the 4 image name along with path and extension: inputs/tajm4.jpg
panorama_image.jpg and matched_points.jpg will be created in output/ folder.
RESULTS
Result of Images from data/tajm folder
tajm1.jpg, tajm2.jpg, tajm3.jpg, tajm4.jpg
