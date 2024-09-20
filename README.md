# Drowsiness-Detection
1. ## **Overview** {#overview}



The primary cause of car accidents is often attributed to poor driving, with factors such as driver fatigue and alcohol consumption playing a significant role in these incidents. Driver fatigue, in particular, is a leading contributor to fatal accidents as it can result in a loss of control while operating a vehicle.

Research findings have indicated that over 20% of all vehicle accidents can be attributed to increased driver fatigue. To address this issue, a project has been initiated with the central objective of developing an eye monitoring system designed to detect signs of driver drowsiness, with the ultimate goal of preventing accidents.

This innovative system will employ contactless technology to assess the driver's attention levels and identify any deficits in their attention while they are behind the wheel. One key aspect of the system's evaluation involves monitoring the duration of eye closure, specifically when the driver's eyes are closed.

If the system detects that the driver's eyes remain closed for an unusually extended period beyond the normal range, it will issue a warning signal, assuming that the driver may have fallen asleep. This system aims to enhance road safety by alerting and preventing accidents caused by driver drowsiness.

2. ## **Motivation** {#motivation}

The motivation behind this report lies in addressing the prevalent issue of car accidents                  
resulting from poor driving, which is often influenced by factors like driver fatigue and   
alcohol consumption. Of these factors, driver fatigue stands out as a significant   
contributor to fatal accidents, primarily due to the loss of control it can induce.

Research has underscored the critical role of driver fatigue, attributing over 20% of all   
vehicle accidents increase tiredness. In response to this problem, a project has been   
initiated with a central objective: the development of an eye monitoring system. This   
system aims to detect early signs of driver drowsiness, ultimately striving to prevent   
accidents on the road.

The innovation at the heart of this project is the use of contactless technology to assess a   
driver's attention levels and identify any lapses in their focus while operating a vehicle.   
A key component of this assessment involves monitoring the duration of eye closure,   
particularly when the driver's eyes are shut.

Should the system detect prolonged eye closure beyond the standard range, it will issue a   
warning signal, presuming that the driver may have fallen asleep. This report seeks to   
motivate the implementation of this system as a means to enhance road safety by   
proactively addressing the issue of driver drowsiness and preventing accidents.

3. ## **Problem Statement and Objectives** {#problem-statement-and-objectives}

The objective of this report is to develop an effective drowsiness detection system using Python, enabling the swift identification of closed eyes to promptly alert drivers when drowsiness is evident. The key to the project's success lies in employing larger datasets and a substantial number of samples, essential for improving system reliability and elevating the accuracy of drowsiness detection. Furthermore, to enhance the performance of the Haar cascade classifier, a streamlined approach involves reducing the number of declared options. This strategy simplifies the system while significantly boosting its capability to accurately identify eye closures associated with drowsiness, making it a valuable tool for ensuring driver safety.

The problem addressed in this report centers on the significant issue of car accidents resulting from factors like poor driving behavior, often influenced by driver fatigue and alcohol consumption. Notably, driver fatigue is a leading cause of fatal accidents due to its potential to result in a loss of control over the vehicle.

Research findings highlight the substantial impact of driver fatigue, attributing over 20% of all vehicle accidents to increased tiredness. In response, this project is initiated with the central goal of developing an eye monitoring system. This innovative system aims to detect early signs of driver drowsiness, ultimately striving to prevent accidents on the road.

A key aspect of the project's innovation is the use of contactless technology to assess a driver's attention levels and identify lapses in their focus during driving, with a particular focus on monitoring the duration of eye closure. When the system detects extended periods of eye closure beyond the standard range, it triggers a warning signal, assuming the driver may have fallen asleep. This report serves as a motivator for implementing the system, enhancing road safety by proactively addressing driver drowsiness and preventing accidents.

4. ## **Details of Hardware/Software Requirement** {#details-of-hardware/software-requirement}

#### **Hardware:**.

* A computer with a dedicated GPU, such as an Nvidia GTX or RTX series graphics card, to run the object detection model efficiently. A GPU with at least 4 GB of VRAM is recommended.

* Sufficient processing power, at least an Intel Core i5 or equivalent processor, to handle the intensive computations required for object detection.

* Sufficient memory, at least 8 GB RAM, to handle the object detection and tracking algorithms.

#### **Software:**

* Operating system: Windows, Linux, or macOS.

* Python 3: To run the project, you will need to have Python 3 installed on your system.

* OpenCV: pip install opencv-python (face and eye detection)

* TensorFlow: pip install tensorflow (keras uses TensorFlow as backend)

* Keras: pip install keras (to build our classification model) 

In addition, you will need a video camera to capture the video stream, or access to a pre-recorded video dataset to test the model.

## **Result Of Our Drowsiness Detection System** {#result-of-our-drowsiness-detection-system}

The model was trained from the dataset after going through all preprocessing and training as shown in Figure 3\. In Figure 1, after successful training, the model was further submitted for computation of the generated loss and accuracy. In early epochs, the training loss was significantly reduced, and eventually the loss was further reduced. Validation started with a small loss, but spikes were observed as it progressed, which leveled off in subsequent epochs. 

![unnamed](https://github.com/user-attachments/assets/fda2f4b9-9fb8-485d-a128-c807a7e7a0c2)


Figure 2 shows the accuracy of the model. Both training and validation show similar accuracy patterns in consecutive epochs, but a larger drop was observed for validation around 40 epochs. The average rated loss was calculated as 0.0550 and the average rated accuracy was calculated as 0.9902. This makes this model the most suitable for use.

![unnamed (1)](https://github.com/user-attachments/assets/4b7e346b-18a1-4966-9dd4-1740df936d69)


This model was derived from other Python guided code that was used to activate a webcam to capture a person in front of a computer system. A new window will open and real time imaging of the person will be captured, as shown in Figure 4\. Data is collected and sent to the model, which analyzes the data and classifies the eye state as 'open' or 'closed'. In Figure 4 the state is shown as Open and the score is shown as 3 because both eyes are open.

![unnamed (2)](https://github.com/user-attachments/assets/37e98abf-987a-4890-9df7-af274c37107c)


Since it is stated that when eyes are open, the lower the score while the higher the score, the more the amount of time the eyes are closed. We see the complement of the previous figure in the next figure. Here (Figure-5) the eyes are closed for a few seconds which led the system to believe that the user was in the state of sleepiness which in turn led the system to increase the score.The system also states that the eyes are in ‘closed’ state while the score is shown to be

![unnamed (3)](https://github.com/user-attachments/assets/f9767830-aa20-46ad-8ae0-8e856ef4f031)




The Purpose of the project is fulfilled as the system is able to differentiate between open and closed eyes in quick time and with good accuracy with low losses. The project further expands the boundaries on the use of real-world data and showing the results in a timely manner. This leads us towards our last chapter of content that will conclude our findings and discuss the potential future of this project.
