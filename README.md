# Squat Counter
> This project counts the number of squats performed by a person in a video.

## Features
##### Main Functionality
This project detects the different body landmarks from the body and then only use the wrist, elbow and shoulder points to calculate the angle between them. On the basis of these angles, system decides if the subject in video is going up or down. 

##### Input
This accepts the video as an input

##### Output
A video with a tally counter integrated into it.

### Coding structure
* Reads the video frame by frame 
* Detects 33 body landmarks using mediapipe model
* Use the coordinates of wrist, elbow and shoulder to determine body position and action
* keep track of actions to determine tally
* write the frames to create a video 

### Directory Structure

    .
    ├── Videos                              # a directory from where the project will read files
        ├── pushup1.MOV
        ├── pushup2.MOV
    ├── output                              # In this directory annotated files produced by the system will be stored
        ├── pushup1_annotated.avi
        ├── pushup2_annotated.avi
    ├── pushups.ipynb                        # a notebook that contains the implementation code
    ├── Antonio-Bold.tff                    # A font style used on videos  
    └── README.md
