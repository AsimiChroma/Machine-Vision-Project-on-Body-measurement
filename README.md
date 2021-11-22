# Limmy-measure-body-dimensions
A small machine vision project that detects and measures the dimensions of a person.

NOTE: Training data not included. If you would like a copy of the training I used, please feel free to contact me!



Project Proposal

Anqi Zhang

CSC592

Description:

My proposal is to find the dimensions of a person's body parts such as
legs, arms, and height, from taking an image of them from a vision system. This is a
useful project because finding the measurements of a person in the clothing industry is
a tedious process and having a system that does that automatically would be extremely
convenient. Of course, there are some apps already out there that do this, but there is
still much to improve on. Most of the apps use pictures taken from a phone, but I want
to go further and try to measure a person’s measurements in real time, with video,
instead of just static pictures. If that is too difficult to be done within the scope of this
project, then I will just try to get the measurements from pictures.

The related topics that will be involved with my project is human detection using
features of the Dalal Triggs pedestrian detector. My goal will be to first locate the person
of question within the image. Aside from just detecting a human I would train the
detector to detect arms and legs as well using a neural network. Most likely I would then
provide images of a Histogram of Gradients using samples from pictures of myself or
from Google to train the neural network to detect these bodily features.

Once the software is able to detect the individual bodily components, I would then use
stereo vision to detect the relative distance of the person from the camera. Since the
distance between the two cameras is known, I can easily calculate the distance of any
point on the image relative to the camera. Using additional computation, I can then
calculate the distance of any two points of a body part to find the dimensions.

The equipment I will mainly be using is a dual camera setup that could support stereo
vision. In particular, I will be using a realsense camera by Intel which has two cameras
built in. I will also be using a computer that can perform the computation and present
the image to the user. Additional resources I may need would possibly be a cloud
database to train the neural network depending on how accurate I want the detection
system to be.


Some references:

● https://medium.com/@xotiv/mobile-apps-can-measure-human-body-measurements-118bc79b48d3

● https://sizer.me/technology/

● https://www.tc2.com/tc2-21b-3d-body-scanner.html
