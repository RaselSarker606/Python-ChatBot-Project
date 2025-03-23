# 🤖 Python Chatbot Project

This Python chatbot built using NLTK and TF-IDF techniques that intelligently responds to user input based on a predefined text file. This project showcases how classic NLP tools can be used to create an interactive chatbot.

---

## 📖 Overview

This project demonstrates a simple rule-based chatbot that:

- Recognizes greetings and common queries  
- Responds using content from a text file  
- Uses TF-IDF and cosine similarity for relevant response generation  

It is ideal for learning how NLP and chatbot logic work at a fundamental level.

---

## 📂 Features

- 🔍 **TF-IDF Matching**: Finds the most relevant response using vector similarity.
- 📄 **Text File as Knowledge Base**: Reads from a plain `.txt` file.
- 🤖 **Greeting Detection**: Responds to greetings like "hi", "hello", and more.
- 🧠 **Smart Response Logic**: Uses cosine similarity for best-match responses.
- 💬 **Interactive Chat Loop**: Lets users chat in real-time until they type "bye".

---

## 🛠️ Methodology

### 🗃️ Dataset Loading
- Reads the content of `DataSci.txt`, which contains the chatbot’s knowledge.

### 🔧 Preprocessing & Tokenization
- Converts text to lowercase.
- Tokenizes the text into sentences and words using `nltk`.

### 👋 Greeting Handling
- Detects and responds to greetings using keyword matching.

### 🧠 Response Generator
- Appends user input to the list of sentences.
- Vectorizes sentences using `TfidfVectorizer`.
- Calculates similarity with `cosine_similarity`.
- Returns the most relevant matching sentence from the knowledge base.

### 🔁 Chat Loop
- Runs until the user types “bye”.
- Handles greetings, thanks, and general questions.

---

## 📊 Example Conversations

```
BOT: I am your chatbot. If you want to exit, type 'bye'

User: Hi  
BOT: hello

User: What is data science?  
BOT: [returns a relevant sentence from DataSci.txt]

User: Thank you  
BOT: You are welcome.

User: Bye  
BOT: Goodbye! Take care.
```

---

## 🚀 Installation & Usage

### 📦 Requirements

- Python 3.x
- NLTK
- Scikit-learn

### 🔧 Setup

```bash
pip install nltk scikit-learn
```

### ▶️ Running the Chatbot

1. Ensure `DataSci.txt` is in the same directory as your script.
2. Run:

```bash
python chatbot.py
```

3. Start chatting in the terminal.

---

## 📌 Future Improvements

- 🧠 Better Context Awareness: Add deeper logic or memory of past messages.
- 🌐 Multilingual Support: Add Bengali and more languages.
- 💻 GUI Integration: Build a simple web or desktop interface.
- 🤖 ML Support: Integrate GPT or transformer-based models for smarter replies.

---

🚀 **Stay tuned for more updates!**
