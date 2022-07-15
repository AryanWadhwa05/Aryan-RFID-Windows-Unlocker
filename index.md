# Raspberry Pi Object Recognition
I am using Raspberry Pi to identify objects through video, webcam, and images. I used TensorFlow Lite to train and run my Object Detection models on the raspberry pi. 

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Aryan | Greenwich High School | Electrical Engineering / Computer Science | Incoming Junior

<br/>

TFLite model             |  My Custom Model
:-------------------------:|:-------------------------:
<img src="https://github.com/AryanWadhwa05/Aryan-BSE-Portfolio/blob/gh-pages/squirrelssample.JPG?raw=true" alt="hi" width="400" height="250"/>  |  <img src= "https://github.com/AryanWadhwa05/Aryan-BSE-Portfolio/blob/gh-pages/Capture.JPG?raw=true" width="400" height="250" />


# Reflection

Throughout my 3 weeks at Bluestamp Engineering, I have learned a great deal in both engineering and coding. I have been taught how to troubleshoot and solve problems by myself. At this summer program, I felt more independent since we were informed by the instructors that they would not provide answers to the students questions unless we have tried at least three different ways to try to solve the problem. I think that Bluestamp’s way of teaching is very unique and promotes students to grasp the art of troubleshooting and solving problems by themselves.

I discovered that both the software and Raspberry Pi aspects of my project were extremely fun and enjoyable to do. From constantly debugging code to setting up my Raspberry Pi, Bluestamp Engineering along with the amazing instructors were able to teach me a great deal through my 3 weeks at the program.

# Showcase Video
This is my demonstration video that was recorded and presented on 7/22/2021. I run through what my project is about, how it works, and what it really does.



# Final Milestone
My final milestone is the implemention of a few object detection model. I used a TensorFlow Lite Model Maker google colab notebook to help guide me upload a object detection dataset and split it into training and testing data. I was able to set up my dataset finding images ont he internet and drawing boxes with labels around the object I want to detect for the computer to recognize. I used and imported the TensorFlow Lite library which makes training and testing a model much easier with only a few lines of code.

```python
#importing all nessecary libraries
import numpy as np
import os

from tflite_model_maker.config import ExportFormat
from tflite_model_maker import model_spec
from tflite_model_maker import object_detector

import tensorflow as tf
assert tf.__version__.startswith('2')

tf.get_logger().setLevel('ERROR')
from absl import logging
logging.set_verbosity(logging.ERROR)

#defining model type from TFLite Model Zoo
spec = model_spec.get('efficientdet_lite2')

#defining training and testing data (importing data)
train_data = object_detector.DataLoader.from_pascal_voc(
    tfrecord_file_patten, size, label_map, annotations_json_file=None
)
validation_data = object_detector.DataLoader.from_pascal_voc(
    tfrecord_file_patten, size, label_map, annotations_json_file=None
)
```

<iframe width="830" height="425" src="https://www.youtube.com/embed/fz4buVoNy_0" title="Final Milestone" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# Second Milestone

My second milestone is detecting object on my Raspberry Pi. I installed mutiple libraries such as TensorFlow and OpenCV to test a TensorFlow Lite pre-trained model on my Raspberry Pi. I downloaded the pre-trained model as detect.tflite from the official Tensor Flow github. I was able to use VNC Viewer to quickly import test images and videos. After that, I was able to run my tflite and Labels file to detect people through my Raspberry Pi camera. I was also able to detect birds and deer through google images.

![Second Milestone Diagram](https://neuralet.com/wp-content/uploads/2020/09/quantization-edge-tpu.png)

<iframe width="830" height="425" src="https://www.youtube.com/embed/hrIigh1v1lc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# First Milestone

My first milestone was setting up and hooking up the Raspberry Pi and all the necessary components onto my monitor/pc. The heatsinks, the sd card, and the nessecary cables were all added to ensure that the Raspberry Pi was working. I downloaded Raspberry Pi imager directly from the official Raspberry Pi website. Raspberry Pi Imager automatically downloads a list of the latest versions of Raspberry Pi OS supported by the Raspberry Pi. The imager allowed me to image Raspian onto the SD card. With the OS imaged onto the SD, I plugged the SD card back into the Raspberry Pi, connected my HDMI cable and rebooted the system until Raspian booted up. I then enabled VNC on the Raspberry Pi so that I was able to use VNC Viewer on my desktop to work on my Raspberry Pi.

<iframe width="830" height="425" src="https://www.youtube.com/embed/D26gl5HK1hM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
