# Driver Drowsiness Detection App

A real-time Driver Drowsiness Detection System that monitors the driver’s alertness using facial analysis. The system triggers audio alerts and sends warnings when signs of drowsiness are detected.
It consists of a Flask-based backend (AI detection) and a Flutter mobile frontend (user interface & alerts).

## Features
### Backend (Flask)

- Real-time eye-blink detection using OpenCV and MediaPipe
- Flask API with /status endpoint returning driver state
- Beautiful UI with status indicators
- Lightweight, designed to run on low-power systems (e.g., Raspberry Pi)

### Frontend (Flutter)
- Real-time drowsiness monitoring
- Audio alerts when drowsiness is detected
- Beautiful UI with status indicators
- Manual alarm control
- Connection status monitoring

## Setup Instructions
###Backend Setup

#### 1. Create a Virtual env and install dependencies

```bash
python -m venv venv
venv\Scripts\activate        # On Windows
pip install -r requirements.txt

```

#### 2. Run the Flask server

```bash
python app.py
```

### Frontend Setup
#### 1. Install dependencies

```bash
flutter pub get
```
#### 2. Run the app
```bash
flutter run
```


## Usage

1. Start your Flask backend server
2. Launch the Flutter app
3. Click "Start Monitoring" to begin drowsiness detection
4. The app will show alerts and play audio when drowsiness is detected
5. Use "Stop Alarm" to manually stop the audio alert

## Troubleshooting

- If you get connection errors, check that your Flask server is running and accessible
- Update the server IP address in the code to match your network
- Ensure the alarm.mp3 file is properly included in assets 
