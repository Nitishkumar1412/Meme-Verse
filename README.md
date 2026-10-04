# 🎭 Meme Verse

Turn your webcam into a meme generator! Make a facial expression or hand gesture, and Meme Verse instantly matches it with a hilarious cat meme—all in real time, directly in your browser.

No uploads, no backend, no installations. Just open the app, allow camera access, and start making faces.

🌐 **Live Demo:** [![Netlify Status](https://img.shields.io/badge/Netlify-Live-00C7B7?logo=netlify&logoColor=white)](https://nitish-meme-verse.netlify.app/)

---

## 🚀 Features

- 📷 Real-time webcam detection
- ✋ Hand gesture recognition
- 😀 Facial expression recognition
- 🎲 Random meme selection based on detected gesture/expression
- 🔄 Prevents consecutive duplicate memes
- ⚡ Fully client-side (your camera feed never leaves your browser)
- 🌙 Responsive and clean UI

---

## 🧠 How It Works

Meme Verse uses **MediaPipe Hands** and **MediaPipe Face Mesh** to detect landmarks from your webcam feed.

The application:

1. Captures live video from your webcam.
2. Detects hand and facial landmarks in real time.
3. Identifies the current gesture or facial expression using landmark geometry.
4. Smooths predictions across multiple frames for stable detection.
5. Displays a matching meme with a smooth transition animation.

Everything runs locally inside your browser—no server processing or image uploads.

---

## 🎯 Supported Gestures & Expressions

| Hand Gestures | Face Expressions |
|--------------|------------------|
| 👍 Thumbs Up | 😊 Smile |
| ✊ Fist | 😝 Tongue Out |
| 👌 OK Sign | 😠 Angry |
| ✌️ Peace | |
| 🤘 Rock | |
| 🤙 Call Me | |
| 🤫 Shh | |

---

## 📁 Project Structure

```
Meme-Verse/
│
├── assets/
│   ├── memes/
│   └── icons/
│
├── gestures.js
├── expressions.js
├── memeManager.js
├── script.js
├── style.css
├── index.html
└── README.md
```

### File Overview

- **gestures.js** – Detects hand gestures using MediaPipe hand landmarks.
- **expressions.js** – Detects facial expressions using MediaPipe face landmarks.
- **memeManager.js** – Loads and displays matching memes while avoiding immediate repeats.
- **script.js** – Controls webcam input, MediaPipe pipeline, prediction smoothing, and UI updates.
- **style.css** – Handles the application's styling and responsive layout.

---

## 🛠️ Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- MediaPipe Hands
- MediaPipe Face Mesh

---

## ⚠️ Limitations

- Works best with a single face and a single hand.
- Performance may vary in poor lighting conditions.
- Extreme camera angles can reduce detection accuracy.
- Gesture recognition is rule-based rather than machine-learning trained.

---

## 📚 Built With

- MediaPipe Hands
- MediaPipe Face Mesh
- Vanilla JavaScript
- HTML & CSS

---

## 🤝 Contributing

Contributions, feature suggestions, and bug reports are always welcome!

If you find an issue or have an idea to improve Meme Verse, feel free to open an issue or submit a pull request.

---

If you found this project interesting, consider giving it a ⭐ on GitHub!
