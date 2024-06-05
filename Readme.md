Problem Statement
As a data scientist at a home electronics company specializing in state-of-the-art smart televisions, your task is to develop an innovative feature that allows users to control the TV through gesture recognition. The system will utilize a webcam mounted on the TV to continuously monitor five distinct gestures, each corresponding to a specific command:

Thumbs up: Increase the volume
Thumbs down: Decrease the volume
Left swipe: Jump backwards 10 seconds
Right swipe: Jump forward 10 seconds
Stop: Pause the movie

Dataset
The dataset consists of a few hundred videos, each categorized into one of the five gesture classes. These videos, typically 2-3 seconds long, are divided into sequences of 30 frames (images). Each video is recorded by different individuals performing one of the five gestures in front of a webcam, simulating real-world usage scenarios.

Data Organization
The data is provided in a zip file containing 'train' and 'val' folders, each accompanied by a CSV file.
Each folder is further divided into subfolders, where each subfolder represents a video of a particular gesture.
Each subfolder contains 30 frames (images) of the video.
CSV File Structure
Each row of the CSV file corresponds to one video and contains:
The name of the subfolder containing the 30 images
The name of the gesture
The numeric label (0-4) of the video
Pre-processing Requirements
Videos are recorded with varying dimensions: 360x360 or 120x160, depending on the webcam used.
Pre-processing is required to standardize the dimensions of the videos.
Objective
Train a model on the 'train' folder that performs well on the 'val' folder. The final model's performance will be evaluated on a withheld 'test' set.

Goal
Develop and implement a robust gesture recognition model that can accurately interpret user gestures, thereby enhancing the user experience by enabling remote-free control of the smart TV. The model should generalize well across different users and varying video dimensions.
