# Drawing-Car-Lanes


### Overview:
This project worked on a video stream that detects lines on the road for a self driving vehicle

### Examples
On an image:

<img src="https://github.com/salarhajimirsadeghi/Drawing-Car-Lanes/blob/master/test_image_output/whiteCarLaneSwitch_output.jpg" width="400">


On a video:

<img src="https://github.com/salarhajimirsadeghi/Drawing-Car-Lanes/blob/master/test_videos_output/solidWhiteRight.gif" width="400">


### Files:
1) In the test_videos_output and test_image_output folders, you'll find the output of the code that was ran in P1.pyn
2) P1.pyn includes all the functions that are needed to manipulate an image or a stream of images (video) in order to detect and draw the lines on the road


### Pipeline:
 My pipeline consisted of 6 steps. 
 1) I converted the images to grayscale
 2) I did a Gaussian Blur to cancel some noise
 3) I used the Canny method to detect edges in our image
 4) I masked the unimportant parts of the image by selecting a portion of our image
 5) I used Hough line transformation to detect the needed lines (road)
 6) Merged our Hough line image with original to see the road on the original image
