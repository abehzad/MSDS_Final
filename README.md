# MSDS_Final

My final project is a combination of image classification and object detection on an iOS edge device. This is a project that starts the process for an object detection app by using CreateML and XCode. CreateML allowed me to train my model, while XCode was used to help deploy my model to an iOS edge device. Currently, my objective is to have this app work on iOS device cameras to detect and classify street signs such as stop, yield, and hazard signs while showing the level of accuracy for each detection. This app can be used to help autonomous vehicles navigate on the streets while abiding by given traffic laws so I hope that this is something that can be used live in a motor vehicle. If a car or autonomous vehicle were using this, it could potentially interact with other systems within the car, such as the braking systems, to help prevent accidents or even deaths.
The overall goal is to combine object detection and image classification to advance and aid drivers and autonomous vehicles in driving safely under various conditions. I find this to be a fun and interesting way to help drivers be safer, while also helping to eliminate human drivers in the future. 

![pic1](abehzad/MSDS_Final/Config/Screen Shot 2020-11-25 at 6.06.48 PM.png)
![GitHub Logo](/images/logo.png)

# Object Detection:
I started testing the idea by classifying the street signs by using IBM’s Cloud Annotation tool. I decided to work with three classes: stop sign, yield sign, and hazard sign. The training dataset is compiled of 100 images of street signs that I could find from Google images both nationally and globally. The validation dataset is compiled of 30 images. I then trained the street sign images through CreateML, which took around 4 hours to complete. Once completed, I tested my model with street sign images that were not in my original dataset. I was able to reach above 97% accuracy across all test images. I decided to work with the Darknet-Yolo model which only views images once. However, such images are scanned by frames per second to make sure there is a high level of accuracy. It took some time to reach this final solution, as I had many failures along the way with other models that either took too long to run or that would crash halfway through. Unfortunately, some models would not mark the street signs correctly within the bounding boxes or would bound other signs if they were within the same image. 


# Conclusion / Future Development:
I was able to test and see my project succeed, which I am very happy about. A few things that I would change for future developments would be having the iOS simulator / app be able to use live video to detect and classify street signs as the camera pans around. This would be extremely helpful in using my device within a human-driven vehicle or driverless car. I have viewed some models that already do that for Formula 1 racing, but they have been developed by Nvidia and other large tech companies. For the time being, I am pleased with my models and results that I have been able to conduct on my laptop and with the given tools (CreateML, Xcode).  
