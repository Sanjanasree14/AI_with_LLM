# AI-Powered Language Learning Chatbot

This project is an **AI-powered grammar and spelling correction chatbot** built using **Streamlit**, **OpenAI GPT-4**, and **SQLite**. The chatbot allows users to input sentences, checks for grammatical errors, categorizes mistakes, and tracks progress over time.

---

## Features
✅ Grammar, spelling, and vocabulary correction using OpenAI GPT-4  
✅ Mistake categorization and storage in SQLite  
✅ Progress tracking with interactive bar charts  
✅ End-of-session summary of mistake trends  
✅ User-friendly **Streamlit UI**  

---

## Installation

1. **Clone the repository:**  
   ```sh
   git clone https://github.com/your-repo/ai-language-chatbot.git
   cd ai-language-chatbot
   ```

2. **Create a virtual environment (Optional but recommended):**  
   ```sh
   python -m venv venv
   source venv/bin/activate   # On Windows use: venv\Scripts\activate
   ```

3. **Install dependencies:**  
   ```sh
   pip install -r requirements.txt
   ```

4. **Set up the OpenAI API key:**  
   - Replace `your-api-key-here` in `app.py` with your OpenAI API key.
   - Or set it as an environment variable:
     ```sh
     export OPENAI_API_KEY="your-api-key-here"
     ```

---

## Usage

Run the chatbot using Streamlit:
```sh
streamlit run app.py
```

Then, open the browser at **http://localhost:8501** to interact with the chatbot.

---

## Database Setup
The chatbot uses **SQLite** to store mistakes for tracking user progress. If you encounter issues with missing columns, you can manually update the database:

1. Open SQLite shell:
   ```sh
   sqlite3 mistakes.db
   ```
2. Add missing columns:
   ```sql
   ALTER TABLE mistakes ADD COLUMN corrected_text TEXT;
   ```
3. Exit the shell:
   ```sh
   .quit
   ```

---

## Future Enhancements
🔹 Voice input for accessibility  
🔹 AI-powered personalized learning recommendations  
🔹 Weekly mistake trends and progress reports  

---
