# Motion and emotion detection

A webcam experiment using OpenCV to detect movement and DeepFace to estimate facial-expression labels.

## Run

Requires Python and an available webcam.

```bash
git clone https://github.com/adjierizqan/Motion-Detection-Emotion-Recognition.git
cd Motion-Detection-Emotion-Recognition
python -m pip install numpy opencv-python deepface
python motion_emotion_detection.py
```

Press `q` to close the webcam window.

The script compares consecutive frames to find movement and uses a face detector before calling DeepFace on each detected face. Model dependencies may download files on the first run.

**Limitations:** The predicted labels describe patterns detected in facial images, not a person's actual feelings. This is a demonstration, not a tool for making decisions about people.

Dependencies are not pinned and there is no automated test setup in this repository.
