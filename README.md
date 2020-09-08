## Color Tracking

This repository is a classic object tracking depending on the color of that object.  

For the ball detection, the image was converted in HSV color palette, in this case the upper and lower bounds were chosing in order to detect a yellow ball and a mask was created from there in order to detect object of interest.  

The limitation of this is project is that at the moment only one object is trackable, the object's color has to be very disctinctive from the background and when encountered with its own reflecction (when the ball is rolling on a bright surface).

## Run code
First activate the virtual environment if you use one, make sure that you have required libraries and there are two possible options to run the script:  

1) Using a previoslly saved video

```bash
python3 path/to/directory/ball_tracking.py --video path/to/video/directory/video.avi
```

2) Using a live webcam

```bash
python3 path/to/directory/ball_tracking.py
```



## Libraries
- cv2
- numpy
- sys
- os
- glob
- imutils
- argparse


## References

The code for the ball detection was based from [here](https://www.pyimagesearch.com/2015/09/14/ball-tracking-with-opencv/). 