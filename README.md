**SignSpeak – Real-Time ISL to Voice Translator**

SignSpeak is a real-time Indian Sign Language translator built using OpenCV for webcam input, MediaPipe for hand-landmark detection, and a CNN-based machine learning model. It recognizes all 26 alphabets (A–Z) along with gestures for space and backspace, converting them into text and speech—essentially enabling “typing” through ISL.

#Dataset & Tools

Dataset: Manually created using a webcam and OpenCV; includes 27 gesture classes (A–Z + Backspace).
Note: Space is detected when no hand is shown for a fixed duration.

Language: Python 3.9.x

Libraries: OpenCV, MediaPipe, TensorFlow/Keras, NumPy, scikit-learn, pyttsx3

Model: Custom CNN

Metrics: Accuracy, Precision, Recall, F1-Score

#How to Run

Install all required Python libraries (tested on Python 3.9.x).

Download the dataset (27 ZIP files) and place them in a folder named data.

If using your own dataset, run createData.py and createBackspace.py instead.

Run preprocess_alphabet.py to generate the landmarks .pickle file.

Train the model using train_alphabet_model.py (default model: CNN; customizable).

Launch test_real_time.py to activate the webcam and begin real-time gesture translation.
