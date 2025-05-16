
# Sign Language Prediction (A–Z)

This project is a real-time sign language alphabet recognition system. It uses your webcam to detect hand gestures and predicts the corresponding American Sign Language (ASL) alphabet using a deep learning model trained on hand landmarks.

## What This Project Does

The system captures hand movements through your webcam, detects key hand landmarks using Mediapipe, and feeds these into an LSTM model trained to recognize letters from A to Z. It’s designed to help bridge communication gaps for those who use sign language.





## Getting Started

**1. Clone this repository to your computer:**

*git clone https://github.com/ZoyaZubair/Sign-Language-Prediction.git*

*cd Sign-Language-Prediction*

**2. Install the required Python packages:**

*pip install opencv-python mediapipe tensorflow numpy*

**3. Collect sign data:**

Run the script to capture images for each letter.

*python collectdata.py*

**4. Extract keypoints from the images:**

*python data.py*

**5. Train the model with the keypoint data:**

*python trainmodel.py*

**6. Run the real-time sign prediction:**

*python app.py*








## How It Works

**1.Hand detection:** Mediapipe locates your hand and tracks landmarks in each frame.

**2.Feature extraction:** These landmarks are saved as arrays for training.

**3.Training:** The LSTM model learns to classify each hand pose as a letter.

**4.Prediction:** In real-time, your webcam feed is processed to identify the letter you’re signing.
## Project Structure

**1. collectdata.py —** script to capture images of hand signs.

**2. data.py —** processes images and extracts hand landmarks.

**3. trainmodel.py —** trains the deep learning model.

**4. app.py —** runs real-time sign prediction using your webcam.

**5. function.py —** contains helper functions for Mediapipe operations.

**6. Image/ —** folder storing raw images.

**7. MP_Data/ —** folder with extracted keypoint data.

**8. model.h5 and model.json —** saved trained model files.


## About Me

I’m Zoya Zubair, passionate about combining AI and computer vision to create practical solutions. Feel free to explore this project and reach out if you have questions or ideas.

Feel free to [connect with me on LinkedIn](https://www.linkedin.com/in/zoya-zubair-62841024b/)!!
