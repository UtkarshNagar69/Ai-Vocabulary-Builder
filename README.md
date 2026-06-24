# AI Vocabulary Builder

An AI-powered vocabulary learning web app that helps users understand English words faster with **meanings, example sentences, synonyms, antonyms, and a quick quiz** — all generated dynamically using AI.

This project is designed to make vocabulary learning more interactive by combining **AI-based word explanations** with a **personal word bank** for revision and practice.

---

## 🚀 Features

- 🔎 **Search any English word**
- 🤖 **AI-generated vocabulary details**, including:
  - Meaning
  - Example sentence
  - Synonyms
  - Antonyms
- 🧠 **Quick fill-in-the-blank quiz** for each searched word
- ⭐ **Save words to a personal Word Bank**
- 💾 **LocalStorage support** to keep saved words in the browser
- ⌨️ **Enter key support** for quick searching
- 🎨 Clean UI using **Tailwind CSS**

---

## 🧠 How It Works

When a user enters a word, the app sends a prompt to an AI model through the **OpenRouter API** and asks for the following in **JSON format**:

- Meaning of the word
- Example sentence
- 3 synonyms
- 3 antonyms
- One fill-in-the-blank quiz with answer

The response is then parsed and displayed on the page in a clean result section.

Users can also save words into a personal **Word Bank**, which is stored in the browser using **localStorage**.

---

## 📌 Core Functionality

### 1. Word Search
Users enter a word into the input field and click **Search** (or press Enter).

### 2. AI Vocabulary Generation
The app uses an AI API call to generate:
- **Meaning**
- **Example**
- **Synonyms**
- **Antonyms**
- **Quiz question + answer**

### 3. Quiz Mode
After generating a word, the app displays a simple quiz to test understanding.

- If the answer is correct → success message
- If incorrect → correct answer is shown

### 4. Save to Word Bank
Users can save words for future revision.  
Saved words are stored in browser **localStorage** under `wordBank`.

---

## 🛠️ Tech Stack

- **HTML5**
- **CSS3**
- **JavaScript (Vanilla JS)**
- **Tailwind CSS**
- **OpenRouter API**
- **LocalStorage**

---

## 📂 Project Structure

```bash
Ai-Vocabulary-Builder/
│
├── index.html          # Main UI of the app
├── script.js           # App logic, API call, quiz logic, localStorage handling
├── style.css           # Custom styles
├── output.css          # Tailwind generated CSS
├── package.json        # Tailwind dependencies
├── package-lock.json
└── README.md
