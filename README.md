# 😊 Text Emotion Detector

A simple web-based **Text Emotion Detection** application that analyzes user-provided text and identifies the dominant emotion using a rule-based Natural Language Processing (NLP) approach.

The application detects emotions such as **Joy, Sadness, Anger, Fear, Surprise, Love, and Neutral** and presents the result through an interactive visual dashboard.

---

## 📌 Project Overview

The **Text Emotion Detector** processes text entered by the user, searches for emotion-related keywords, calculates emotion scores, and determines the dominant emotion.

It is designed as an educational NLP project that demonstrates how text can be analyzed using JavaScript without requiring external APIs or machine-learning services.

---

## 🎯 Objectives

* Detect emotions from text.
* Demonstrate basic Natural Language Processing concepts.
* Calculate emotion scores using predefined keywords.
* Display the dominant emotion visually.
* Show emotion confidence and percentage breakdown.
* Maintain recent analysis history using LocalStorage.
* Provide a simple and responsive user interface.

---

## ✨ Features

* 😊 Joy detection
* 😢 Sadness detection
* 😡 Anger detection
* 😨 Fear detection
* 😲 Surprise detection
* ❤️ Love detection
* 😐 Neutral classification
* 📊 Emotion percentage breakdown
* 📈 Confidence meter
* 📝 Character counter
* 🕘 Recent analysis history
* 💾 LocalStorage support
* 🔄 Clear and reset option
* 📱 Responsive design
* 🎨 Pastel emotion-based dashboard

---

## 🛠️ Technologies Used

* **HTML5** — Structure
* **CSS3** — Styling and responsive design
* **JavaScript** — Emotion analysis and application logic
* **LocalStorage** — Storing recent analysis history
* **NLP Concepts** — Keyword-based emotion classification

---

## 🧠 How It Works

The application follows these steps:

```text
User enters text
        ↓
Text preprocessing
        ↓
Convert text to lowercase
        ↓
Remove unnecessary punctuation
        ↓
Split text into words
        ↓
Compare words with emotion dictionary
        ↓
Calculate emotion scores
        ↓
Find dominant emotion
        ↓
Calculate confidence
        ↓
Display result
        ↓
Save analysis history
```

---

## 🔍 Emotion Categories

| Emotion     | Example Keywords                            |
| ----------- | ------------------------------------------- |
| 😊 Joy      | happy, excited, amazing, wonderful, success |
| 😢 Sadness  | sad, lonely, crying, disappointed, hopeless |
| 😡 Anger    | angry, furious, hate, frustrated, unfair    |
| 😨 Fear     | afraid, scared, nervous, danger, panic      |
| 😲 Surprise | surprised, shocking, unexpected, wow        |
| ❤️ Love     | love, adore, caring, beautiful, romantic    |
| 😐 Neutral  | Text with no strong emotion keywords        |

---

## 🧮 Emotion Scoring

Each emotion-related word has a predefined score.

For example:

```text
happy     → Joy +3
excited   → Joy +3
sad       → Sadness +3
angry     → Anger +3
scared    → Fear +3
surprised → Surprise +3
love      → Love +3
```

The application adds the scores and selects the emotion with the highest score.

---

## 🔄 Negation Handling

The application also includes basic negation handling.

For example:

```text
"I am happy."
```

can produce:

```text
Joy
```

Whereas:

```text
"I am not happy."
```

can reduce or reverse the emotion score because the system checks for words such as:

* not
* never
* no
* don't
* didn't
* isn't
* can't

This provides a basic demonstration of contextual text processing.

---

## 📊 Example

### Input

```text
I am extremely happy and excited about my success!
```

### Output

```text
😊 Joy

Confidence: High
```

Another example:

### Input

```text
I feel lonely and disappointed today.
```

### Output

```text
😢 Sadness
```

---

## 📁 Project Structure

```text
TextEmotionDetector/
│
├── index.html
└── README.md
```

The entire application is contained inside a single HTML file containing:

* HTML
* CSS
* JavaScript

---

## 🚀 How to Run in VS Code

### Step 1 — Create Folder

Create a folder named:

```text
TextEmotionDetector
```

### Step 2 — Open in VS Code

Open the folder in Visual Studio Code.

### Step 3 — Create File

Create:

```text
index.html
```

### Step 4 — Paste Code

Paste the complete Text Emotion Detector code into `index.html`.

### Step 5 — Run

You can either:

* Open `index.html` directly in your browser, or
* Use the **Live Server** extension in VS Code.

### Step 6 — Test

Enter a sentence and click:

```text
Detect Emotion
```

---

## 💾 LocalStorage

The application stores the latest five analyses in the browser.

Storage key:

```text
emotionHistory
```

The stored information includes:

* Text
* Detected emotion
* Analysis time

No external database is required.

---

## 🔐 Privacy

This project processes the entered text locally in the browser.

It does not send the entered text to an external server or API.

However, recent analyses are stored in the browser's LocalStorage.

---

## ⚠️ Limitations

This project uses **rule-based emotion detection**, so it is not equivalent to a trained machine-learning or large language model.

It may have difficulty understanding:

* Sarcasm
* Complex sentences
* Slang
* Multiple emotions in one sentence
* Cultural expressions
* Context-dependent meanings
* Unknown words
* Very subtle emotions

For example:

```text
"Yeah, great job breaking everything."
```

could be misunderstood because sarcasm is difficult for keyword-based systems.

---

## 🔮 Future Enhancements

The project can be upgraded with:

* Machine Learning emotion classification
* Python NLP backend
* Natural Language Toolkit (NLTK)
* Transformer-based models
* AI API integration
* Multilingual emotion detection
* Speech emotion detection
* User accounts
* Cloud database
* Emotion history charts
* Real-time analysis
* Sentiment + emotion combined analysis

---

## 🎓 Academic Applications

This project can be used for:

* NLP mini projects
* Web technology projects
* Artificial Intelligence demonstrations
* Human-computer interaction projects
* Text analysis experiments
* CSE laboratory demonstrations
* Mini project presentations

---

## 📚 Concepts Demonstrated

* Natural Language Processing
* Text preprocessing
* Keyword classification
* Score-based classification
* Basic negation handling
* JavaScript DOM manipulation
* Event handling
* LocalStorage
* Responsive web design
* Data visualization using progress bars

---

## 🧪 Sample Test Cases

| Input                               | Expected Emotion |
| ----------------------------------- | ---------------- |
| I am very happy today!              | 😊 Joy           |
| I feel lonely and hurt.             | 😢 Sadness       |
| I am extremely angry.               | 😡 Anger         |
| I am scared of the situation.       | 😨 Fear          |
| Wow! This is completely unexpected! | 😲 Surprise      |
| I love my family so much.           | ❤️ Love          |
| The class starts at 10 AM.          | 😐 Neutral       |

---

## 👩‍💻 Author

**Charulatha S**

B.E. Computer Science Engineering
Prathyusha Engineering College

---

## 📌 Project Series

This project is:

**Application 2 of 10 — Text & Speech Analysis Applications**

### Series

1. ✅ Text Sentiment Analyzer
2. ✅ **Text Emotion Detector**
3. ⏳ Text Statistics Analyzer
4. ⏳ Keyword & Topic Extractor
5. ⏳ Text Summarizer
6. ⏳ Speech-to-Text Analyzer
7. ⏳ Speech Emotion Analyzer
8. ⏳ Voice Command Application
9. ⏳ Speech Characteristics Analyzer
10. ⏳ Text & Speech Chat Assistant

---

## ⭐ Conclusion

The **Text Emotion Detector** demonstrates how basic NLP techniques can be used to identify emotions from written text.

Although it uses a rule-based approach, it provides a simple foundation for understanding **text preprocessing, emotion classification, scoring, and visualization** and can later be extended into a machine-learning or cloud-based NLP application.
