# Face Puzzle Game

A modern browser-based Face Puzzle Game that uses your webcam to capture a photo and instantly transform it into a draggable jigsaw-style puzzle.

## Features

### Camera Capture

* Uses `getUserMedia()` to access the webcam
* Front-facing camera preferred on mobile devices
* Live camera preview before capture
* One-click photo capture
* Graceful handling of camera permission denial
* Works on HTTPS or localhost

### Puzzle Generation

* Create puzzles from your captured photo
* Multiple difficulty levels:

  * 3 × 3 (9 pieces)
  * 4 × 4 (16 pieces)
  * 5 × 5 (25 pieces)
* Automatically slices the captured image into puzzle tiles
* Randomized puzzle layout
* Solvable puzzle generation

### Drag & Touch Controls

* Desktop mouse drag support
* Mobile touch gesture support
* Drag-and-drop tile swapping
* Automatic snapping to puzzle grid
* Visual drag feedback
* Correctly positioned tiles highlighted in green

### Game Statistics

* Live timer display
* Move counter
* Correct pieces tracker
* Difficulty indicator
* Real-time progress updates

### Results & Leaderboard

* Automatic win detection
* Results modal upon completion
* Displays:

  * Completion time
  * Total moves
  * Difficulty level
* Local leaderboard storage using `localStorage`
* Top 5 best scores saved
* Leaderboard includes:

  * Date
  * Time
  * Moves
  * Difficulty

### Responsive Design

* Mobile-friendly layout
* Tablet support
* Desktop support
* Modern UI
* Touch-optimized controls

---

## Browser Compatibility

Supported browsers:

* Google Chrome
* Mozilla Firefox
* Safari
* Microsoft Edge

Camera functionality requires:

* HTTPS connection
* OR localhost during development

---

## How to Play

1. Allow camera access when prompted.
2. Position your face within the camera preview.
3. Click **Take Photo**.
4. Choose a difficulty level.
5. Start the puzzle.
6. Drag puzzle pieces to swap positions.
7. Complete the image to win.
8. Compare your score on the leaderboard.

---

## Controls

### Desktop

* Click and drag a puzzle piece.
* Drop it onto another piece to swap positions.

### Mobile / Tablet

* Touch and hold a puzzle piece.
* Drag to another location.
* Release to swap pieces.

---

## Game Flow

1. Camera Access
2. Take Photo
3. Select Difficulty
4. Generate Puzzle
5. Solve Puzzle
6. View Results
7. Save Score
8. Play Again or Capture New Photo

---

## Project Structure

Single-file application:

```text
index.html
├── HTML Markup
├── Embedded CSS
└── Embedded JavaScript
```

No build tools required.

No frameworks required.

No external backend required.

---

## Technologies Used

* HTML5
* CSS3
* JavaScript (ES6+)
* Canvas API
* MediaDevices API
* LocalStorage API
* Pointer Events / Touch Events

---

## Security & Privacy

* Images remain on the user's device.
* No photo uploads occur.
* No external image processing.
* No personal data is transmitted.
* Leaderboard data is stored locally in browser storage.

---

## Installation

Simply open the HTML file in a supported browser.

For camera access:

```bash
# Option 1
Serve via HTTPS

# Option 2
Run locally
http://localhost
```

Example:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

---

## Future Enhancements

* Share scores
* Online leaderboard
* Puzzle piece animations
* Multiple puzzle shapes
* Image upload option
* Dark/Light themes
* Achievement system
* Sound effects

---

## License

Free to use for personal and educational projects.
