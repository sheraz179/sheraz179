# A web app to track a person
> This project tracks a person which is selected by a user in a provided video and then calcualtes
  it's similarity with a benchmark video using pose points.

## Features
##### Main Functionality
> User can upload a new benchmark/challenge against which he wants to find simialrities for a person of his own choosing
> User can delete a benchmark
> User can view a benchmark video and all compared videos

##### Input
> This accepts the video as an input

##### Output
> A tracked video
> A pose points file
> DTW score against a challenge.

### Directory Structure
        
        ├── detectron2-windows          # a directory containing detectron 2 code
        ├── dynamic_time_wraping
            ├── __init__.py
            ├── dtw.py
        ├── routers                     # a directory that contains different routers regarding the fastapi
            ├── benchmark.py            #contain end-points to process the benchmark video
            ├── track_person.py         #contain end-points to process the video for tacking
        ├── static
            ├── challenge1
                ├── benchmark           # contain all data related with a benchmark
                    ├── video_name      # an uploaded file
                    ├── benchmark.mp4   # A tracked video
                    ├── pose_points.csv # contains the pose points of a tracked person
                ├── pose points         # contains detected pose points of all videos
                ├── uploaded videos     # videos that were uploaded for tracking
                ├── tracked videos      # tracked videos
                ├── dtw_scores          # contains calculated dtw scores of tracked videos witha benchmark video
        ├── templates
            ├── index.htm               #home page template
            ├── benchmark.htm           #a template to add new benchmark to database
            ├── preview.htm             #displays the first frame from where a user can select the person to track
            ├── benchmark_videos.htm    #templates to display vidoes under a specific challenge along with their scores
            ├── delete_benchmark.htm    #a template to delete the benchmark
                
        ├── utils
            ├── utils.pt               # This contains the utility functions
        ├── config.py
        ├── main.py 
        └── README.md
        
        
