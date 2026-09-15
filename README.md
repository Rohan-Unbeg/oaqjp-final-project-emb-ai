# Emotion Detector

Final project for the IBM course "Developing AI Applications with Python and Flask".

An AI based web application that detects the emotions expressed in a piece of text. It uses the Watson NLP EmotionPredict service to score the text for anger, disgust, fear, joy and sadness, reports the dominant emotion, and serves the result through a Flask web interface.

## Project structure

- `EmotionDetection/emotion_detection.py`: the `emotion_detector` function that calls Watson NLP and formats the result
- `EmotionDetection/__init__.py`: makes `EmotionDetection` an importable package
- `test_emotion_detection.py`: unit tests for the emotion detector
- `server.py`: Flask server that deploys the application
- `templates/index.html`, `static/mywebscript.js`: the web interface

## Running

```
pip install flask requests
python3 server.py
```

Then open http://localhost:5000 and enter text to analyze.
