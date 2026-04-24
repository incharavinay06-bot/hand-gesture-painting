Gesture Paint — Touchless Drawing using Computer Vision

Overview

Gesture Paint is a real-time, touchless drawing application that allows users to draw on screen using only hand gestures. It uses computer vision to track hand movements via a webcam and translates them into drawing actions.
This project removes the need for a mouse, stylus, or touchscreen, making interaction more intuitive and futuristic.


Features

- Draw in the air using hand gestures  
- Real-time hand tracking using MediaPipe  
- Multiple tools:
  - Freehand drawing
  - Line
  - Rectangle
  - Circle
  - Eraser  
- Color selection panel (Blue, Green, Red)  
- Hover-based selection (no clicking required)  
- Visual feedback with blinking pointer  
- Smooth real-time performance  

---

 Tech Stack

- Python  
- OpenCV  
- MediaPipe  
- NumPy  


How It Works

1. Webcam captures live video feed  
2. MediaPipe detects hand landmarks  
3. Finger positions are analyzed:
   - Index finger → selection mode  
   - Index + middle finger → drawing mode  
4. Hovering over UI elements selects tools/colors  
5. Drawing is rendered onto a virtual canvas  


Controls & Gestures

| Gesture | Action |
|--------|--------|
| Index Finger Up | Move pointer / Select |
| Index + Middle Up | Draw |
| Hover on tool | Select tool |
| Hover on color | Change color |
| `Q` key | Quit |
| `F` key | Toggle fullscreen |


Installation

1. Clone the repository
```git clone https://github.com/your-username/gesture-paint.git```
cd gesture-paint

2. Install dependencies
pip install opencv-python mediapipe numpy

4. Run the project
python main.py
Project Structure
gesture-paint/
│
├── main.py
├── README.md
└── requirements.txt (optional)

Use Cases

  Computer vision learning projects
  Gesture-based UI research
  Touchless interaction systems
  Creative digital drawing

Future Improvements

  Add more colors and brush sizes
  Save/export drawings
  Undo/Redo functionality
  Multi-hand tracking
  Advanced gesture controls
