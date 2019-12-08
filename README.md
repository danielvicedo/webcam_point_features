# webcam_point_features
Detection of ORB features from online webcam images.

Forked repository: https://github.com/beta-robots/webcam_point_features

Added a factor variable which multiplies by the width and height of the image and limits the size of the area of the mask.

Added a mask where keypoints are found only in a part of the whole image.

#ORB features (Oriented FAST and rotated BRIEF)

ORB is an alogithm created to search for keypoints in images using FAST in pyramids to detect stable keypoints, selects the strongest features using FAST or Harris response, finds their orientation using first-order moments and computes the descriptors using BRIEF (where the coordinates of random point pairs are rotated according to the measured orientation).

It is as an efficient and viable alternative to SIFT and SURF. ORB was conceived mainly because SIFT and SURF are patented algorithms. ORB, however, is free to use.

ORB builds on the well-known FAST keypoint detector and the BRIEF descriptor. Both of these techniques are attractive because of their good performance and low cost. ORB’s main contributions are as follows:

- The addition of a fast and accurate orientation component to FAST
- The efficient computation of oriented BRIEF features
- Analysis of variance and correlation of oriented BRIEF features
- A learning method for decorrelating BRIEF features under rotational invariance, leading to better performance in nearest-neighbor applications


Bibliography:

- https://medium.com/@deepanshut041/introduction-to-orb-oriented-fast-and-rotated-brief-4220e8ec40cf?
- https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_feature2d/py_orb/py_orb.html
