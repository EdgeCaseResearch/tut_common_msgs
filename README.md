# Tut Common Messages

Common ROS messages used for TUT. These are desiged to be pulled by every SUT and are a common way for TUT and each SUT to communicate.

The repon contains a ROS action, `CheckForObjects`, that takes an image and an ID and returns a set of bounding boxes and classification probabilities for all objects found in the image, as well as a results image that shows the classified results. 

SUTs should be able to handle this action, receiving an image, parsing their internal results and returning bounding boxes and a results image. 
