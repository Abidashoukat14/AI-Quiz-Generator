# 🤖 AI-Powered Quiz Generator Using Together API

A smart and interactive quiz generation system designed for **teachers** and **students**. This project uses the **Together API** to create dynamic quizzes based on uploaded PDF notes. It can generate multiple question types and adjust difficulty levels in real-time for personalized learning.

---

## 📚 Project Overview

This AI tool performs two primary roles:

* 👩‍🏫 **Teacher Mode**: Generates customizable quizzes (MCQs, Fill in the Blanks, True/False) with or without answers.
* 👩‍🎓 **Student Mode**: Provides quiz questions and evaluates user answers dynamically with increasing difficulty.

The system processes **PDF notes** using NLP techniques and generates quizzes via **Together API's Llama-2 model**.

---

## ✨ Key Features

* 🔍 Extracts text automatically from uploaded PDFs
* 🧠 Generates context-based questions using AI
* 🎯 Multiple question types: MCQs, Fill in the Blanks, True/False
* 🧪 Separate quizzes with and without answers
* 📈 Adaptive difficulty adjustment in Student Mode
* 💾 Downloadable quiz files (text format)

---

## 🧑‍🏫 For Teachers

1. Upload your lecture PDF.
2. Choose difficulty level.
3. Select number of questions for each type.
4. Click **Generate Quiz**.
5. View and download quiz (with and without answers).

---

## 👨‍🎓 For Students

1. Upload your PDF notes.
2. Select initial difficulty level.
3. Start the quiz.
4. Answer questions one by one.
5. View correct answers and track your performance.
6. Quiz difficulty adapts based on your results.

---

## 📁 Project Structure

```
├── app.py                 # Streamlit frontend for Teachers & Students
├── project.py             # CLI version for quiz generation
├── Api.py                 # File containing the Together API Key
├── requirements.txt       # Dependencies
├── quiz_questions.txt     # Output file (without answers)
├── quiz_with_answers.txt  # Output file (with answers)
```

---

## 🛠 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/Abidashoukat14/ai-quiz-generator.git
cd ai-quiz-generator
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Set Up API Key

Create a file named `Api.py` and add your Together API key:

```python
apikey = "your_together_api_key_here"
```

Or, add it in your `.env` file:

```env
TOGETHER_API_KEY=your_together_api_key_here
```

### 4. Run the App

```bash
streamlit run app.py
```

---

## 💡 How It Works

* `PdfReader` extracts text from PDFs
* `ask_together_api()` communicates with the Together API to get AI-generated questions
* Questions are cleaned with regex to remove answers (for student use)
* Quiz files can be downloaded or viewed directly in Streamlit

---

## 🔮 Future Enhancements

* ✅ GUI quiz-taking timer and score visualization
* ✅ Teacher panel for quiz history management
* ✅ Quiz export to PDF or Google Forms
* ✅ Login authentication for role-based access

---

## 🎓 Author

**Abida Shoukat**
📧 [LinkedIn Profile](https://www.linkedin.com/in/abida-shoukat-a5518831b)


---


## 🙌 Contributions

Pull requests and ideas are welcome! Let's make AI quiz generation easier for educators and learners.

---

