# **SignSpeak – Real-Time Indian Sign Language (ISL) Translator**


SignSpeak is a real-time ISL-to-Text-and-Voice translation system built using OpenCV, MediaPipe, and a CNN-based gesture recognition model. It recognizes all 26 alphabets (A–Z) along with gestures for Space and Backspace, allowing users to “type” using ISL and convert it into both text and audio output.

# **✨ Features**


Real-time gesture recognition using a webcam

Hand landmark detection via MediaPipe

Custom CNN achieving high accuracy on a 27-class dataset

Converts recognized signs into text and speech

Supports Space and Backspace gestures for smooth typing experience

# **📁 Dataset**

Dataset created manually using webcam + OpenCV

Total 27 classes (A–Z + Backspace)

Note: “Space” is detected automatically when no hand is visible for a set duration

Dataset included as 27 ZIP files

Alternatively, you can generate your own dataset using the provided scripts

# **🛠️ Tech Stack**

Programming Language: Python 3.9.x

Libraries: OpenCV, MediaPipe, TensorFlow/Keras, NumPy, scikit-learn, pyttsx3

Model Used: CNN

Evaluation Metrics: Accuracy, Precision, Recall, F1-score

# **🚀 How to Run**

Install all required Python libraries (tested on Python 3.9.x).

Download and extract the 27 ZIP files into a folder named data/.

If generating your own dataset, run:

createData.py

createBackspace.py

Run preprocess_alphabet.py to generate the landmarks .pickle file.

Train the model using train_alphabet_model.py.

Run test_real_time.py to start the webcam and translate gestures in real time.
