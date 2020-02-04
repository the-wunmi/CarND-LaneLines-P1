# **Finding Lane Lines on the Road** 

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[solidYellowCurve_gray]: ./test_images_output/solidYellowCurve_gray.png
[solidWhiteCurve_gray]: ./test_images_output/solidWhiteCurve_blur.png
[whiteCarLaneSwitch_gray]: ./test_images_output/whiteCarLaneSwitch_gray.png
[solidYellowLeft_gray]: ./test_images_output/solidYellowLeft_gray.png
[solidWhiteRight_gray]: ./test_images_output/solidWhiteRight_gray.png

[solidYellowCurve_blur]: ./test_images_output/solidYellowCurve_blur.png
[solidWhiteCurve_blur]: ./test_images_output/solidWhiteCurve_blur.png
[whiteCarLaneSwitch_blur]: ./test_images_output/whiteCarLaneSwitch_blur.png
[solidYellowLeft_blur]: ./test_images_output/solidYellowLeft_blur.png
[solidWhiteRight_blur]: ./test_images_output/solidWhiteRight_blur.png

[solidYellowCurve_canny_edge]: ./test_images_output/solidYellowCurve_canny_edge.png
[solidWhiteCurve_canny_edge]: ./test_images_output/solidWhiteCurve_canny_edge.png
[whiteCarLaneSwitch_canny_edge]: ./test_images_output/whiteCarLaneSwitch_canny_edge.png
[solidYellowLeft_canny_edge]: ./test_images_output/solidYellowLeft_canny_edge.png
[solidWhiteRight_canny_edge]: ./test_images_output/solidWhiteRight_canny_edge.png

[solidYellowCurve_roi]: ./test_images_output/solidYellowCurve_roi.png
[solidWhiteCurve_roi]: ./test_images_output/solidWhiteCurve_roi.png
[whiteCarLaneSwitch_roi]: ./test_images_output/whiteCarLaneSwitch_roi.png
[solidYellowLeft_roi]: ./test_images_output/solidYellowLeft_roi.png
[solidWhiteRight_roi]: ./test_images_output/solidWhiteRight_roi.png

[solidYellowCurve_hough]: ./test_images_output/solidYellowCurve_hough.png
[solidWhiteCurve_hough]: ./test_images_output/solidWhiteCurve_hough.png
[whiteCarLaneSwitch_hough]: ./test_images_output/whiteCarLaneSwitch_hough.png
[solidYellowLeft_hough]: ./test_images_output/solidYellowLeft_hough.png
[solidWhiteRight_hough]: ./test_images_output/solidWhiteRight_hough.png

[solidYellowCurve]: ./test_images_output/solidYellowCurve.png
[solidWhiteCurve]: ./test_images_output/solidWhiteCurve.png
[whiteCarLaneSwitch]: ./test_images_output/whiteCarLaneSwitch.png
[solidYellowLeft]: ./test_images_output/solidYellowLeft.png
[solidWhiteRight]: ./test_images_output/solidWhiteRight.png
---

## Reflection

My pipeline consisted of 5 steps:

##### 1. Converted original image to a grayscale image

![alt text][solidYellowCurve_gray] ![alt text][solidWhiteCurve_gray] ![alt text][whiteCarLaneSwitch_gray] ![alt text][solidYellowLeft_gray] ![alt text][solidWhiteRight_gray]

##### 2. Applied a Guassian blur to smoothen edges and reduce noises.

![alt text][solidYellowCurve_blur] ![alt text][solidWhiteCurve_blur] ![alt text][whiteCarLaneSwitch_blur] ![alt text][solidYellowLeft_blur] ![alt text][solidWhiteRight_blur]

##### 3. Applied canny edge detection

![alt text][solidYellowCurve_canny_edge] ![alt text][solidWhiteCurve_canny_edge] ![alt text][whiteCarLaneSwitch_canny_edge] ![alt text][solidYellowLeft_canny_edge] ![alt text][solidWhiteRight_canny_edge]

##### 4. Derive region of interest from a polygonal shape

![alt text][solidYellowCurve_roi] ![alt text][solidWhiteCurve_roi] ![alt text][whiteCarLaneSwitch_roi] ![alt text][solidYellowLeft_roi] ![alt text][solidWhiteRight_roi]

##### 5. Use Hough Transform to trace out lanes within the derived region of interest.

![alt text][solidYellowCurve_hough] ![alt text][solidWhiteCurve_hough] ![alt text][whiteCarLaneSwitch_hough] ![alt text][solidYellowLeft_hough] ![alt text][solidWhiteRight_hough]

##### Final Result

![alt text][solidYellowCurve] ![alt text][solidWhiteCurve] ![alt text][whiteCarLaneSwitch] ![alt text][solidYellowLeft] ![alt text][solidWhiteRight]

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
