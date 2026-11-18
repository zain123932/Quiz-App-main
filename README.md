# Quiz App

A responsive, timer-based quiz application built with **HTML, CSS and vanilla JavaScript**. Players answer multiple-choice questions against a 15-second countdown, get instant feedback on every answer, and see a final score at the end.

**Live Demo:** https://zain123932.github.io/Quiz-App-main/

---

## Features

- Start screen showing the total number of questions and the time limit
- 15-second countdown timer for every question
- Instant feedback: the chosen answer turns red or blue, and the correct answer is always revealed
- Animated progress bar and question counter (e.g. `3 / 7`)
- Final result screen with score percentage, correct answers and wrong answers
- One-click restart
- Fully responsive layout for desktop and mobile
- Dark theme with glow effects and smooth animations
- No frameworks, no dependencies, no build step

## Tech Stack

| Technology | Purpose |
|------------|---------|
| HTML5 | Page structure |
| CSS3 | Styling, animations, responsive layout (Flexbox, media queries) |
| JavaScript (ES6) | Quiz logic, timer, DOM manipulation |
| Google Fonts (Nunito) | Typography |

## Project Structure

```
quiz-app/
├── index.html    # Markup: start screen, quiz box, result screen
├── style.css     # All styling and animations
├── script.js     # Quiz data and application logic
└── README.md     # Project documentation
```

## Getting Started

No installation is required.

1. **Clone the repository**
   ```bash
   git clone https://github.com/zain123932/quiz-app.git
   ```
2. **Open the project folder**
   ```bash
   cd quiz-app
   ```
3. **Run it**
   Open `index.html` in any modern browser, or use the *Live Server* extension in VS Code.

## How It Works

1. The player clicks **Start Quiz** and the first question loads.
2. A 15-second timer starts. If it reaches zero, the correct answer is revealed automatically.
3. Clicking an option locks all buttons, marks the answer as correct or wrong, and updates the score.
4. **Next** moves to the following question.
5. After the last question, the result screen shows the score as a percentage along with correct and wrong counts.

## Adding Your Own Questions

Questions live in the `quizData` array at the top of `script.js`. Add a new object to extend the quiz:

```js
{
  question: "Which language runs in the browser?",
  options: ["Python", "JavaScript", "C++", "Java"],
  answer: "JavaScript"
}
```

The `answer` value must match one of the `options` exactly. The total question count on the start screen updates automatically.

## Customization

- **Time per question:** change `timeLeft = 15` in `script.js` (and the label in `index.html`).
- **Colors and theme:** edit the colors in `style.css`.
- **Number of options:** each question can have any number of options.

## Roadmap

- [ ] Count unanswered (timed-out) questions as wrong
- [ ] Shuffle questions and options
- [ ] Save the high score with `localStorage`
- [ ] Review screen showing missed questions
- [ ] Category and difficulty selection
- [ ] Sound effects

## Author

**Zain**
Software Engineering Student

- GitHub:[@zain123932](https://github.com/zain123932)
