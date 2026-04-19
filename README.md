# ✋ Air Draw — Hand Tracking Canvas

Draw anything in the air using just your webcam and your hand!  
Built with **MediaPipe** + **OpenCV**.

---

## 🎥 Features

| Feature | How it works |
|---|---|
| **Air Drawing** | Point your index finger and move it — lines appear on screen |
| **Pen Up / Pen Down** | Pinch your index finger & thumb together to lift the pen |
| **Distance Scaling** | Move your hand **closer** → brush gets **bigger**; move **away** → smaller |
| **Two-hand Scale** | Use both hands — the distance between index fingers controls scale |
| **Undo** | Press `Z` to remove the last stroke |
| **Color Picker** | Press `B` to cycle through 8 colors (including an eraser) |
| **Brush Sizes** | Press `1`–`5` for preset sizes |
| **Save Drawing** | Press `S` to export your art as a PNG |

---

## 🚀 Quick Start

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/air-draw.git
cd air-draw
```

### 2. Create a virtual environment (recommended)
```bash
python -m venv venv
source venv/bin/activate      # macOS / Linux
venv\Scripts\activate         # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run!
```bash
python air_draw.py
```

---

## 🕹️ Controls

| Key | Action |
|---|---|
| Index finger | Draw on canvas |
| Pinch (index + thumb) | Lift pen (stop drawing) |
| Move hand closer/farther | Scale brush up / down |
| `B` | Next color |
| `1` – `5` | Brush size (tiny → huge) |
| `Z` | Undo last stroke |
| `C` | Clear canvas |
| `S` | Save as PNG (→ `saves/` folder) |
| `R` | Reset distance scale reference |
| `Q` / `Esc` | Quit |

---

## 🖐️ Hand Gestures

```
Index finger up, others down → DRAWING mode
         ✌ pinch              → PEN UP (stop line)
Two hands in frame           → Scale mode (spread = zoom in)
```

---

## 🗂️ Project Structure

```
air-draw/
├── air_draw.py        # Main application
├── requirements.txt   # Python dependencies
├── saves/             # Auto-created when you save a drawing
└── README.md
```

---

## 📦 Requirements

- Python 3.8+
- Webcam
- `opencv-python` ≥ 4.8
- `mediapipe` ≥ 0.10
- `numpy` ≥ 1.24

---

## 💡 Tips

- **Good lighting** helps MediaPipe detect your hand reliably.
- Keep your hand roughly **40–80 cm** from the camera for best tracking.
- Use **slow, deliberate movements** for clean strokes.
- The **scale reference** is set the first time a hand is detected — press `R` to reset it.

---

## 📄 License

MIT — do whatever you want with it!
