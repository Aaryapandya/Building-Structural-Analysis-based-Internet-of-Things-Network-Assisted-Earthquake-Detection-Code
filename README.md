# Building Structural Analysis based on Internet of Things Network assisted Earthquake Detection

The paper is published in the Internet of Things Volume 19, August 2022, by Elsevier.
https://www.sciencedirect.com/science/article/abs/pii/S2542660522000579

# Introduction
Earthquakes are one of the most devastating geohazards in the world. The effects of earthquakes can be annihilating, causing widespread loss of life and property, and indirectly affecting the country's economy. Analysing the patterns of these earthquakes and creating a system to detect them, can help to minimize loss of lives. Existing sensor-based detection works failed to distinguish between earthquakes and other external vibrational noises that may be caused due to construction or other external sources. In the proposed work, to overcome this drawback, the first in-depth structural analysis of shear walls is done to find a structurally suitable location to install the sensor in a building. Further, the MPU6050 sensor is used to reduce the complexity and make the circuit less bulky. This sensor consists of an accelerometer which measures the change in acceleration and a gyroscope which records the shaking pattern of the ground. Since this shaking pattern is exhibited exclusively by an earthquake occurrence, the proposed model distinguishes between the earthquake and other non-hazardous vibrations efficiently. With the considered model for machine learning algorithms, we were able to achieve 99.82% of accuracy, which is a crucial factor for earthquake detection.

# Motivation
An earthquake is the shaking of the surface of the Earth resulting from a sudden release of energy in the Earth's lithosphere that creates seismic waves. This causes mass destruction in its magnitude. When an earthquake occurs then normally this brings many natural calamities. When this comes near human settlement then this may take humans life. There are lots of human losses due to earthquakes. Sometimes it may introduce other disasters such as landslides, and tsunamis that may also disrupt human life. Living in Himachal Pradesh, I have observed very closely that earthquake occurs frequently compared to the rest of the country.

# Technology Used
a)	Internet of Things
The MPU 6050 is connected to Arduino, and communication is done through the I2C protocol. As MPU6050 supports only I2C communication, hence, it must be connected only to the I2C pins of the Arduino. For collecting the data sets, the setup consisting of the sensors was mounted on a wooden platform. A hand drill was used to create vibrational tremor patterns, while the shaking patterns were created manually and partly due to the wooden platform being loose on the ground. MPU6050 sensor was interfaced with the Arduino Uno R3, having an accelerometer and a gyroscope-accelerometer to measure the acceleration of tremors and to measure the magnitude of the shift in orientation respectively. The sensor is then ready to transmit data and can be used in the detection of externally stimulated tremors and shaking patterns as its dataset is to be collected. The created IoT dataset consists of 59,276 total readings of 3-dimensional coordinates of accelerometer and gyroscope, of which, 30,598 are earthquakes and 28,678 are non-earthquakes This labelled data is then sent to machine learning models for training.
b)	Machine Learning and Deep Learning
2 Machine Learning Models were used, Logistic Regression and Support Vector Machine. Receiver Operating Characteristic Curve (ROC) and the area under its curve (AUC) are used to compare the two algorithms. To get higher accuracy we used a deep learning model with 2 dense layers to avoid overfitting of data.

# Result
Earthquakes are one of the most catastrophic natural disasters in the world. In the project, an IoT network-based study related to earthquake detection has been performed. Most of the previously existing models failed to distinguish between earthquakes and other external vibrational noise that may be caused due to construction or other external sources. The first in-depth structural analysis of the building where sensors have to be placed is done. Then various sensors and their properties and effectiveness in earthquake detection are explained in detail. Three models of machine learning - Logistic Regression, SVM and CNN were used and it was concluded that the CNN model gave the highest accuracy and precision.

