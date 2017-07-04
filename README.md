# **Finding Lane Lines on the Road** 

## Writeup Template

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
---


### 1. Pipeline 
 My pipeline consisted of 6 steps. 
 1) I converted the images to grayscale
 2) I did a Gaussian Blur to cancel some noise
 3) I used the Canny method to detect edges in our image
 4) I masked the unimportant parts of the image by selecting a portion of our image
 5) I used Hough line transformation to detect the needed lines (road)
 6) Merged our Hough line image with original to see the road on the original image

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

Here is an image example:

![alt text](https://github.com/salarhajimirsadeghi/Drawing-Car-Lanes/blob/master/test_image_output/whiteCarLaneSwitch_output.jpg)

Here is a video example:
![alt text](https://github.com/salarhajimirsadeghi/Drawing-Car-Lanes/blob/master/test_videos_output/solidWhiteRight.gif)


### 2. Shortcomings with my current pipeline


One potential shortcoming would be when the roads get twisty and windy, I don't think my pipeline can detect all the lines property. 


### 3. Improvements to my pipeline

A possible improvement would be to better my slope function that's derived from hough lines function, 
