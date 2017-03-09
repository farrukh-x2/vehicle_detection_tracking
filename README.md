## Vehicle Detetction and Tracking

This project is based on writing a software pipeline to detect and track vehicles in a video. Output is shown below:

![](vehicle_detection_tracking.gif)

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
* `test_images` contains example images for testing the pipeline on single frames.
* `test_video.mp4` is a test video to check the performance of pipeline.
* `test_video_output.mp4` is the result of pipeline on the `test_video.mp4`.
* `project_video.mp4` is the main input video the pipeline works on.
* `vehicle_detection_tracking` files contain the output. the mp4 is the original video and gif is displayed above:

Notebook
---
The `vehicle_detection_and_tracking.ipynb` notebook goes through each of the steps laid out above with accompanying images
