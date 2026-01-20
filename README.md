# AI Chatbot Using NLP and Arithmetic Evaluation

A lightweight, offline AI chatbot built using Natural Language Processing (NLP) techniques.  
The chatbot is capable of engaging in basic conversational dialogue and accurately solving simple arithmetic queries, while keeping the total project size under **100 MB**.

---

## 📌 Project Overview

This project focuses on designing and implementing a **compact AI chatbot** that can:
- Understand user intent from natural language input
- Respond appropriately to conversational queries
- Perform arithmetic calculations such as addition, subtraction, multiplication, and division
- Run **offline**, without relying on internet access or large language models

The chatbot uses **intent classification** powered by pre-trained word embeddings and a lightweight neural network, combined with a secure math expression evaluator.

---

## 🎯 Objectives

- Build an NLP-based chatbot capable of simple human-like conversation
- Implement intent recognition using neural networks
- Integrate arithmetic query solving in natural language (e.g., *“What is 3 plus 4?”*)
- Keep the system lightweight and efficient (<100 MB)
- Ensure the chatbot works offline and is easy to deploy

---

## ✨ Final Features

The final version of the chatbot includes:

### 🗣 Conversational Capabilities
- Greetings and farewells
- Polite responses and courtesy replies
- Jokes and small talk
- Handling of inappropriate or irrelevant input
- Self-aware responses (basic personality)

### 🧮 Arithmetic Evaluation
- Supports natural language math queries:
  - `What is 3 plus 4?`
  - `10 divided by 2`
  - `5 * 6`
- Converts word-based operators (plus, minus, divided by) into symbols
- Uses a **safe AST-based evaluator** to prevent malicious execution

### 🧠 NLP & Machine Learning
- Intent classification using:
  - Tokenization and padding
  - Pre-trained **GloVe 6B (50d) embeddings**
  - Lightweight neural network architecture
- Trainable embeddings for better adaptation on small datasets
- Confidence-based intent selection with fallback responses

### 🖥 User Interface
- Simple **Tkinter-based popup chat window**
- Separate GUI window (not terminal-based)
- User-friendly text input and scrollable chat history

### 📦 Lightweight Design
- GloVe embeddings trimmed to ~60–70 MB
- Compact trained model (~10–20 MB)
- Entire project comfortably under **100 MB**

---

## 🏗 System Architecture

User Input
↓
Text Preprocessing (tokenization, padding)
↓
Intent Classification (Neural Network)
↓
┌───────────────┬─────────────────┐
│ Math Query? │ Conversational │
│ → Evaluate │ → Select Reply │
└───────────────┴─────────────────┘
↓
Bot Response


---

## 🛠 Technologies Used

- **Programming Language:** Python
- **Libraries & Frameworks:**
  - TensorFlow / Keras
  - NumPy
  - NLTK
  - Tkinter
- **Embeddings:** GloVe 6B (50-dimensional)
- **Development Environment:** VS Code (Jupyter Notebook)
- **Testing Environment:** Google Colab

---

## 📂 Project Structure (Typical)

AI-Chatbot-Using-NLP/
│
├── intents.json # Intent dataset
├── embeddings/
│ └── glove_70mb_50d.txt # Trimmed GloVe embeddings
├── model/
│ └── chatbot_model.h5 # Trained model
├── chatbot_notebook.ipynb # Main notebook (training + inference)
├── gui.py / gui cell # Tkinter chatbot window
├── README.md
└── report/
└── AI_Chatbot_MiniProject_Report.pdf


---

## 🧪 Sample Interactions

User: Hi
Bot: Hello human

User: Tell me a joke
Bot: A vampire bat arrives back at the roost...

User: What is 3 plus 4?
Bot: 3 + 4 = 7

User: Bye
Bot: Goodbye, have a nice day!


---

## ⚠️ Limitations

- No long-term conversational memory
- Limited to predefined intents
- Not a knowledge-based or generative AI system
- English language only

---

## 🚀 Future Enhancements

- Expand intent dataset for richer conversation
- Add contextual memory for multi-turn dialogue
- Support multiple languages
- Deploy as a web or mobile application
- Integrate syllabus or domain-specific query modules

---

## 📚 References

- Jurafsky, D., & Martin, J. H. *Speech and Language Processing*
- Manning, C. D., & Schütze, H. *Foundations of Statistical NLP*
- Stanford GloVe Embeddings  
  https://nlp.stanford.edu/projects/glove/
- TensorFlow Documentation  
  https://www.tensorflow.org/

---

## 👤 Author

**Abuzaid Khan**  
Final-Year Engineering Student  
AI & NLP Enthusiast

---

⭐ If you find this project useful, feel free to star the repository!
