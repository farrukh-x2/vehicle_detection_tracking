## Vehicle Detetction and Tracking

In this project, the goal is to write a software pipeline to detect vehicles and track them in a video

The Project
---

The goals / steps of this project are the following:

* Perform a Histogram of Oriented Gradients (HOG) feature extraction on a labeled training set of images and train a classifier Linear SVM classifier
* For those first two steps we normalize the features and randomize a selection for training and testing.
* Implement a sliding-window technique and used trained classifier to search for vehicles in images.
* Run pipeline on a video stream (first with the test_video.mp4 and later implemented on full project_video.mp4) and create a heat map of recurring detections frame by frame to reject outliers and follow detected vehicles.
* Estimate a bounding box for vehicles detected.

Usage
---
The training data used to train the classifier can be found for [vehicle](https://s3.amazonaws.com/udacity-sdc/Vehicle_Tracking/vehicles.zip) and [non-vehicle](https://s3.amazonaws.com/udacity-sdc/Vehicle_Tracking/non-vehicles.zip) examples  .  These example images come from a combination of the [GTI vehicle image database](http://www.gti.ssr.upm.es/data/Vehicle_database.html), the [KITTI vision benchmark suite](http://www.cvlibs.net/datasets/kitti/)
Cloning the repository and downloading the above files will make the notebook work

Files
---
Some example images for testing the pipeline on single frames are located in the `test_images` folder.  The video called `project_video.mp4` is the video the pipeline works on. `test_video_output.mp4` is the application of the pipeline on the `test_video.mp4`

`vehicle_detection_tracking` files contain the output. the mp4 is the original video and gif is displayed below:

![](vehicle_detection_tracking.gif)

Notebook
---
The `vehicle_detection_and_tracking.ipynb` notebook goes through each of the steps laid out above with accompanying images
