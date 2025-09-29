## This is the folder for running the OpenCV trackers (Boosting, MIL, KCF, TLD, Medianflow, MOSSE, CSRT)

### How to run the different trackers:
- To run any of them, you simply run the command: `python3 all_the_trackers.py`, which will run whichever tracking algorithm is chosen in the code
- In order to change the algorithm you want to run, simply go to line 12 in `all_the_trackers.py` and change `tracker_types[6]` to match the algorithm you want:
  - `tracker_types[0]` = Boosting
  - `tracker_types[1]` = MIL
  - `tracker_types[2]` = KCF
  - `tracker_types[3]` = TLD
  - `tracker_types[4]` = Medianflow
  - `tracker_types[5]` = MOSSE
  - `tracker_types[6]` = CSRT

### What do all of these trackers have in common?
They are classical single-object trackers, which means they only detect an object's motion between frames. "But why does that matter? Isn't that what a tracker does?" 
Yes, but when it comes to scenarios where an object leaves the view of the camera, even for a split second, these tracking algorithms suddenly stop working and render themselves mostly useless.


So how do we fix this? That's where detection and deep learning come into play, which we will learn more about in the next tracking algorithm: YOLO + DeepSORT.
