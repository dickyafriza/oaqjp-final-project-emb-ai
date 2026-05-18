# Final Project

**Project Name:** Final Project

An emotion detection web application built using **Watson NLP Library** and **Flask**. This project analyzes text input and detects emotions — anger, disgust, fear, joy, and sadness — identifying the dominant emotion.

## Project Details

| Item | Detail |
|------|--------|
| **Course** | Developing AI Applications with Python and Flask (IBM / Coursera) |
| **Type** | Final Project |
| **API** | Watson NLP Embeddable AI — EmotionPredict |
| **Framework** | Flask (Python) |
| **License** | Apache 2.0 |

## Features

- 🔍 **Emotion Analysis** — Detects 5 emotions (anger, disgust, fear, joy, sadness) from text input
- 🏆 **Dominant Emotion** — Identifies the strongest emotion in the text
- 🌐 **Web Interface** — Flask-based UI for easy interaction
- ⚠️ **Error Handling** — Gracefully handles blank/invalid input
- ✅ **Unit Tested** — 5 test cases covering all emotion categories
- 📊 **Code Quality** — Pylint score: **10.00/10**

## Project Structure

```
emotion_detection/
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
├── static/
│   └── mywebscript.js
├── templates/
│   └── index.html
├── server.py
├── test_emotion_detection.py
├── README.md
└── LICENSE
```

## Setup & Usage

### Prerequisites
- Python 3.10+
- IBM Skills Network Cloud IDE (for Watson NLP API access)

### Installation

```bash
git clone https://github.com/<your-username>/emotion_detection.git
cd emotion_detection
pip install flask requests
```

### Run the Application

```bash
python server.py
```

Open your browser at `http://localhost:5000`

### Run Unit Tests

```bash
python -m unittest test_emotion_detection.py
```

### Run Static Code Analysis

```bash
pylint server.py
```

## API Endpoint

| Method | Endpoint | Parameter | Description |
|--------|----------|-----------|-------------|
| GET | `/` | — | Renders the web interface |
| GET | `/emotionDetector` | `textToAnalyze` | Returns emotion analysis result |

### Example Response

```
For the given statement, the system response is 'anger': 0.01, 'disgust': 0.02,
'fear': 0.03, 'joy': 0.82, 'sadness': 0.05. The dominant emotion is joy.
```
