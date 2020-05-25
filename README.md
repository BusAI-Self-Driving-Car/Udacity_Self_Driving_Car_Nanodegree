# Udacity Self-Driving Car Nanodegree Course

In this repo, it contains the projects I worked on for the Self-Driving Car Nanodegree Course on Udacity.  Each course is separated into directories.  For each directory, a clone from the relevant repo is made, followed by the necessary edits required to constitute a complete submission for that project.  You may consult each directory for the instructions for that particular project for more details.

## Python Dependencies
* `moviepy`
* `opencv-python`
* `tensorflow` - Note that the course uses version 1.x but I will be using 2.x.  Keras has been folded into Tensorflow from 2.0 and onwards so there's no need to install Keras separately.
* `numpy`
* `matplotlib`
* `pandas`
* `python-socketio`
* `eventlet`
* `pillow`
* `flask`
* `aiohttp`

These can be installed through `pip` with the `requirements.txt` file included with this repo:

```sh
$ pip install -r requirements.txt
```

## Project #1 - Simple Lane Finding Algorithm

This directory contains a method using simple computer vision algorithms to help localise where lanes are with respect to the ego vehicle.  Given sample images from the front camera of a car on a highway, we determine the left and right lanes for the car.  Please navigate to the `CarND-LaneLines-P1` directory for more details.  The report can be found in this directory under `reflection_report.md`.

## Project #2 - Advanced Lane Finding Algorithm

This directory contains a method using more advanced computer vision algorithms to help localise where lanes are with respect to the ego vehicle.  The objective and criteria for performance evaluation are the same as Project #1.  Please navigate to the `CarND-Advanced-Lane-Lines-P2` directory for more details.  The report can be found in this directory under `reflection_report.md`.

## Project #3 - Traffic Sign Classification Algorithm

This directory contains a method using deep learning to classify traffic sign images.  We specifically explore the dataset used for training this system and provide an architecture that performs the classification well on the training, validation and test dataset.  Please navigate to the `CarND-Traffic-Sign-Classification-Project-P3` directory for more details.  The report can be found in this directory under `final_report.md`.

**Note:**  The dataset is not stored on this repo, but it can be downloaded yourself.  Open up the notebook file in the  `CarND-Traffic-Sign-Classification-Project-P3` directory and run the cells that are relevant to downloading the data.

## Project #4 - Behaviour Cloning Algorithm

This directory contains a method using deep learning to output the steering angle for a car to ensure it stays on the road given a front-facing camera image.  The data to collect was from a simulator provided by Udacity where we capture front-facing camera images as well as the steering angle so that we can train a deep neural network.  This will be directly substituted into the simulator to see if we can autonomously keep the car on the road.  Please navigate to the `CarND-Behavioral-Cloning-P4` directory for more details.  The report can be found in this directory under `final_report.md`.

**Note:** As of this writing, the provided simulator on https://github.com/udacity/self-driving-car-sim does not run on Mac OS Catalina.  Fortunately, there were efforts made to rebuild the simulator on Catalina and can be retrieved here: https://github.com/endymioncheung/CarND-MacCatalinaSimulator.  Just in case this repo no longer exists, I have forked it here: https://github.com/rayryeng/CarND-MacCatalinaSimulator.

**Note #2:** The model was trained using Google Colab Pro, so there is a training notebook you can examine to see how the model was trained.  In addition, the dataset used for training this model is not available on this repo due to size constraints.  It is hosted on my personal Dropbox so you can run the cell in the notebook to download it on your computer if you so desire.

**Note #3:** Be advised that Tensorflow 2.0 was used to train this model.  The course uses TF 1.x with Keras 2.x using TF as the backend.  TF and Keras were separated in older versions of the software.  As of TF 2.0, Keras was eventually integrated into TF.