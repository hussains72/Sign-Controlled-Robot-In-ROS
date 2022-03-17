# Sign-Controlled-Robot-In-ROS
This project is about controlling robot motion with hand gestures which have commands like rotate, move forward and backward, accelarate and stop.The project have two parts :

Detection of Hand_Gesture using opencv library.

Integrating Hand_Gesture to publish commands to robot.

# Algorithm
# ALORITHM FOR DETECTION OF HAND_GESTURE

Seperate out the skin color from the input frame using HSV or other color format with upper and lower bound for skin color as per range. Removal of noise from image via Morphological Transformation, and applying filters to smooothen the image.Finding the contour of the mask and finding its convex-hull.
Using the various properties for seperation various Hand_Gestures(In this project we will use Indian-sign-language as Hand_Gesture- 1,2,3..) like- convexity defects along with contour properties like solidity, extent and aspect ratio of respective gesture.
