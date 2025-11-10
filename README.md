# 🎯 Simple Quiz App

A lightweight, interactive **Quiz Application** built using **HTML**, **CSS**, and **JavaScript (ES Modules)**.  
It dynamically loads questions, tracks scores, and provides instant feedback on each answer — perfect for learning fundamentals or as a base for more advanced quiz systems.

---

## 🚀 Features

- 🎨 **Clean, Responsive UI** — Built with pure CSS, fully mobile-friendly  
- ⚡ **Dynamic Question Loading** — Questions imported from external JS files  
- ✅ **Instant Feedback** — Correct/Incorrect highlights for each answer  
- 🔁 **Play Again Option** — Restart the quiz without reloading the page  
- 🧠 **Score Tracking** — Displays final score after the last question  

---

## 📂 Project Structure

```
quiz-app/
│
├── index.html          # Main HTML structure
├── style.css           # Styling and responsive layout
├── script.js           # Core quiz logic and DOM manipulation
└── questions/
    └── q1.js           # Question set exported as a JS module
```

---

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/atharvashirodkar/quiz-app.git
   cd quiz-app
   ```

2. **Open the app locally:**
   - Use any **local server** (e.g., VS Code Live Server)
   - Or open `index.html` directly in your browser

3. **Project uses ES modules**, so make sure you’re running it from a server environment, not just `file://`.

---

## 🧩 Usage Example

Add questions inside `questions/q1.js` like this:

```js
const questions = [
  {
    question: "What is the capital of France?",
    answers: [
      { text: "Paris", correct: true },
      { text: "Rome", correct: false },
      { text: "Madrid", correct: false },
      { text: "Berlin", correct: false }
    ]
  },
  {
    question: "Which language runs in a web browser?",
    answers: [
      { text: "Python", correct: false },
      { text: "C++", correct: false },
      { text: "JavaScript", correct: true },
      { text: "Java", correct: false }
    ]
  }
];

export default questions;
```

Then import it inside `script.js`:
```js
import questions from "./questions/q1.js";
```

---

## 🧠 How It Works

- Loads questions dynamically from the imported JS module  
- Displays each question with multiple answer buttons  
- Highlights selected answers (green/red) and tracks the score  
- After all questions, shows the final score and a "Play Again" option  

---

## 💬 Support & Feedback

If you encounter bugs or have feature suggestions:
- Open an issue in the repository’s **Issues** tab  
- Or start a discussion in **Discussions**  

For setup help, check:
- [CONTRIBUTING.md](CONTRIBUTING.md)

---

## 👥 Maintainers & Contributions

**Maintainer:** [atharvashirodkar](https://github.com/atharvashirodkar)  
Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) before submitting pull requests.

---

## 🪪 License

This project is licensed under the terms of the [MIT License](LICENSE).

---
