# Speed_breaker_detection_for_Indian_roads

Road safety has recently received a lot of attention and accidents brought on by speeding have resulted in severe loss of life and property. The excessive use of speed breakers on national highways has become a major issue as it can cause accidents and loss of lives. Drivers often fail to recognize the appearance of unmarked speed breakers and lose control of their vehicles, resulting in serious accidents. Moreover, sudden deceleration or acceleration caused by speed breakers can also
damage vehicles. The failure to notice speed breakers on the roadways is one of the causes of such incidents. The Regionbased Convolutional Neural Network (RCNN) architecture, deep learning, and image processing are used in this paper to provide a unique technique for speed breaker identification. The proposed system uses a camera mounted on a moving vehicle to take pictures of the roadways, which are then processed to look for potential speed bumps. The prospective speed limiters are then
categorised using the RCNN model, along with their precise location on the route. The results show that the proposed system can accurately detect speed breakers with good precision and recall rates on a collection of road photos collected from diverse locations. The suggested method can be utilised in real-time to
warn drivers of approaching speed limits and avoid collisions brought on by speeding. This method has the ability to greatly decrease the frequency of accidents on the road and improve traffic safety.





# METHODOLOGY

A. MODEL TRAINING

We are using a deep learning network for speedbreaker detection. For this, we are using a fast RCNN architecture. An early warning system is used to alert the driver in advance when the vehicle is approaching a speed breaker. To collect the information about speed breakers, an autonomous data collection module has been developed where the iterative speed behavioral patterns of vehicles are analyzed and probable locations for the speed breakers are identified. Here, speed breakers are clustered into routes according to their longitude and latitude values. Based on the collected data, speed breakers are detected and a warning message is generated. The algorithm used for speedbreaker detection is Fast-RCNN. Fast R-CNN passes the entire image to ConvNet, which generates regions of interest (instead of passing the extracted regions from the image). 
It uses a single model that extracts features from the regions, classifies them into different classes, and returns the bounding boxes. All these steps are done simultaneously, thus making it execute faster as compared to R-CNN. Faster R-CNN fixes the problem of selective search by replacing it with the Region Proposal Network (RPN).
Faster R-CNN has two networks: A region proposal network (RPN) for generating region proposals and a network for detecting objects using these proposals. 
1. Take an input image and pass it to the ConvNet, which returns feature maps for the image.
2. Apply Region Proposal Network (RPN) on these feature maps and get object proposals.
3. Apply ROI pooling layer to bring down all the proposals to the same size.
4. Finally, pass these proposals to a fully connected layer in order to classify any predicted bounding boxes for the image.

![Fast-RCNN-framework-for-object-detection-and-classification](https://github.com/Vipul1019/Speed_breaker_detection_for_Indian_roads/assets/77145832/b838f71b-292c-421c-863d-3bbafc7e1a92)


B. Speed breaker Detection Module:

The Region-based Convolutional Neural Network (RCNN) architecture is then employed for classification and localization after potential speed bumps have been identified. In several computer vision applications, object detection and localization have been accomplished using the deep learning model RCNN.
The RCNN model extracts characteristics from each ROI using a convolutional neural network after segmenting the image into distinct regions of interest (ROI). The class of the object is then determined using these features, and its location is determined using a bounding box regressor. The speed breakers in the road photos are classified and located using the RCNN model, which is trained on a dataset of speed breaker images in the proposed system. To strengthen the system, the training dataset contains pictures of speed bumps taken at various angles and in various lighting situations. Once trained, the RCNN model may be used to analyse images taken by the camera installed on the moving vehicle in order to detect speed bumps in real-time. The technology can help prevent accidents brought on by speeding and increase road safety by warning the motorist of impending speed breakers in real-time. In conclusion, the proposed system for speed breaker detection combines image processing, deep learning, and the RCNN architecture to effectively identify and localise possible speed breakers. This approach has the potential to greatly reduce the amount of traffic accidents brought on by speed limit enforcement and increase road safety.

<img width="580" alt="flowchartspeeed" src="https://github.com/Vipul1019/Speed_breaker_detection_for_Indian_roads/assets/77145832/fc35e30e-8711-4e3a-9d68-a7a5c285c9dc">

# RESULTS 

Obtained Loss after 4 epochs = 0.0138

<img width="304" alt="res" src="https://github.com/Vipul1019/Speed_breaker_detection_for_Indian_roads/assets/77145832/1d6521df-bc81-44df-a793-4e4db4120467">




