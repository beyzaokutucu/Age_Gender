# Gender and Age Detection

## About the Project :
This project utilizes OpenCV and Deep Learning to accurately detect a person's age and gender from a single image of their face. The program can process both single images and video streams, providing age and gender predictions for each individual.

In this Python project, I employed Deep Learning techniques to precisely determine a person's gender and age based on a single facial image. I utilized models trained by Tal Hassner and Gil Levi for this purpose. The predicted gender can be either 'Male' or 'Female', and the predicted age falls into one of the following ranges: (0 – 2), (4 – 6), (8 – 12), (15 – 20), (25 – 32), (38 – 43), (48 – 53), (60 – 100) (with 8 nodes in the final softmax layer).

Accurately estimating an exact age from a single image is challenging due to various factors such as makeup, lighting conditions, obstructions, and facial expressions. Therefore, I formulated this as a classification problem rather than a regression one.
## Additional Python Libraries Required :
- OpenCV 


```   pip install opencv-python ```


-argparse 


```  pip install argparse ```


## The contents of this Project :
- opencv_face_detector.pbtxt
- opencv_face_detector_uint8.pb
- age_deploy.prototxt
- age_net.caffemodel
- gender_deploy.prototxt
- gender_net.caffemodel
- a few pictures to try the project on
- detect.py <br/>


For face detection, we have a .pb file- this is a protobuf file (protocol buffer); it holds the graph definition and the trained weights of the model. We can use this to run the trained model. And while a .pb file holds the protobuf in binary format, one with the .pbtxt extension holds it in text format. These are TensorFlow files. For age and gender, the .prototxt files describe the network configuration and the .Working: file defines the internal states of the parameters of the layers. <br/>


 ## Working:
 
![İmages](https://github.com/beyzaokutucu/Age_Gender/blob/main/Age_Gender/Example/example.png)
## Examples :
 
```
Gender: Female  
Age: 25-32 years
```


![İmages](https://github.com/beyzaokutucu/Age_Gender/blob/main/Age_Gender/Example/example2.png) <br>


## Examples :
```
Gender: Female
Age: 25-32 years
```
