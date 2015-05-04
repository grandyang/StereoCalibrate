# StereoCalibrate
Calibration of stereo pair of the images

Modification based on Martin Peris's work

http://blog.martinperis.com/2011/01/opencv-stereo-camera-calibration.html

Usage: 
StereoCalibrate filename nx ny squareSize

Example:
StereoCalibrate list.txt 9 6 2.5

Paremeters:
filename   - A list that contain all the pair images, the total number of images should be even.
nx         - Number of horizontal squares
ny         - Number of vertical squares
squareSize - Size of square

Note:
- nx, ny should be set correctly according to the checkerboard, if not, no correct results will get.
- All the corners in the checkerboard in each image should be detected.
- If the final average error is below 1.0, it indicates a good calibration. If not, please adjust the positions and orientations of the checkerboard. (For how to get a good calibration, please check Martin Peris's blog)
- (http://blog.martinperis.com/2011/01/opencv-stereo-camera-calibration.html)
