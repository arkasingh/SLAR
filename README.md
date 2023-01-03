# Sign Language Action Recognition

This project makes use of Google mediapipe holistic for data processing and Long Short-Term Memory (LSTM) neural network architecture built on TensorFlow Keras for real-time sign action recognition achieving an accuracy of 98.67%.

The computer vision library OpenCV was utilized to record over 5 different American Sign Language (ASL) gestures namely “yes”, “no”, “hello”, “thank you” and “nice to meet you”. Every gesture was recorded 100 times with 30 frames in each sequence. The data pre-processing required generating the landmark points for face, hands and pose, each point defined by their position in 3D space with an additional visibilty dimension in pose landmarks. Total 1662 such features were extracted from each frame of the recorded sequences and saved in NumPy arrays.

**Gestures**

*Yes*

![yes](https://user-images.githubusercontent.com/110922376/210288940-d4a215ca-8d98-4b4c-9ab1-e7f27bb6de08.gif)

*Hello*

![hello](https://user-images.githubusercontent.com/110922376/210289010-7750aa89-dd79-445a-a48c-e6cf45d0c60e.gif)

*No*

![no](https://user-images.githubusercontent.com/110922376/210289021-a2fffe85-75f6-49b0-b679-78a12c2ea368.gif)

*Thank You*

![ThankYou](https://user-images.githubusercontent.com/110922376/210289038-40c395a6-4c66-4b04-a2d3-cc7f17d03c8e.gif)

*Nice To Meet You*

![NiceToMeetYou](https://user-images.githubusercontent.com/110922376/210289052-da944e7b-d0b4-425c-911c-86954bc7b082.gif)

The two jupyter notebooks are given as: *Sign Action Detection Project Demo.ipynb* file, for demonstrating how frames were captured using OpenCV with keypoints marked using mediapipe, and *Sign Language Gesture Recognition Project.ipynb* file as the main project having all the neccesary code for capturing the said 5 gestures and then implemneting it for the action recognition LSTM training network.

The saved weight of the LSTM network with the data used in this project is given as *lstm_sign_action.h5*. It can be used as a base model for further finetuning the nectwork with gestures by different people with varied body languages captured in different lighting set up for better generalization.
