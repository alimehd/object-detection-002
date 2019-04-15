# Object recognition app with Tensorflow, OpenCV and Flask

This is the code for an oject detection app that is hosted on Heroku as  the backend engine.
 The app is using [Tensorflow Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection),
 OpenCV and Flask. You can find it at the following link:

https://mehdidetection.herokuapp.com/

### TensorFlow model
Google has released some pre-trained models for object recognition in an image. Here, ssd mobilenet model is used. It 
is a model trained on the COCO dataset.

### Model implementation

1. User uploads a image as a file through the form provided by the flask app on Heroku.
2. Upon sumitting the request, the image is used as the input for the model.
3. The frozen model is loaded into the memory.
4. The detection code is being run and the objects are being detected and labeled.