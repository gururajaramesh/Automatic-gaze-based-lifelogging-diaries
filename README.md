# Automatic gaze-based lieflogging/diaries
Designing a model that can recognize a person’s day-to-day activities accurately is a challenging task. In this project, we propose a model that gives the life-log of a person’s activities in a day into 9 different categories (outdoor, social interaction, focused work, travel, reading, computer work, watching media, eating, special) with inputs as multi-channel time series signals procured from long term video recordings which has been recorded by an eye tracker and a scene camera. First, we extract frames from the video, and we generate optical flow image for every extracted frame. Then, features are extracted from both the raw images and their corresponding optical flow image by a pre-trained VGG16 model. Then the features from VGG16 and the gaze data are given to a LSTM layer where the final activities are predicted. We also have an alternative model where we use only the raw frames and gaze data for activity recognition.
## Key Concepts used for the project
* VGG16
* Convolutional Neural Networks
* Long Short Term Memory Networks(LSTM)

## Libraries Used
* Keras Functional API
* Flownet 2.0
* Numpy
* other common Deep learning libraries