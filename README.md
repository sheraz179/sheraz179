# Squat Counter
> This project counts the number of squats performed by a person in a video.

## Features
##### Main Functionality
This project detects the different body landmarks from the body and then only use the ankle, knee and hip points to calculate the angle between them. On the basis of these angles, system decides if the subject in video is going up or down. 

##### Input
This accepts the video as an input

##### Output
A video with a tally counter integrated into it.

## Developing

Here's a brief intro about what a developer must do in order to start developing
the project further:

### Directory Structure

├── Videos                  # a directory from where the project will read files
    ├── squat_side.MOV
    ├── squat_front.MOV
├── output                  # output videos will be stored here
    ├── squat_side_annotated.avi
    ├── squat_front_annotated.avi
├── squats.ipynb                     # a notebook that contains the implementation code
├── Antonio-Bold.tff        # A font style used on videos                  
└── README.md
