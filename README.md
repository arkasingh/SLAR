# Sign Language Action Recognition

This project makes use of Google mediapipe holistic for data processing and Long Short-Term Memory (LSTM) model for real-time sign action recognition achieving an accuracy of 98.67%.

The computer vision library OpenCV was utilized to record over 5 different American Sign Language (ASL) gestures namely “yes”, “no”, “hello”, “thank you” and “nice to meet you”. Each video sequence comprised of 30 frames was recorded and 100 such video sequences were captured for each gesture to be utilized as train and test data. The data pre-processing required generating the landmarks for face, hands and pose and saving the data in NumPy arrays.

