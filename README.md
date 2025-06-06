# 🧠 Therapy Session Analyzer

A human-centered NLP dashboard that helps therapists detect and visualize emotional patterns in session notes using AI. Powered by state-of-the-art transformer models and built with a clean Streamlit interface, this tool supports mental health professionals by transforming unstructured text into emotional insights.

---

## 📌 Project Highlights

> "When emotions speak, our system listens."

- 🎯 Tracks emotional trends across therapy sessions  
- 🧠 Uses AI models to detect sadness, joy, fear, etc.  
- 🔐 Secure login for therapists  
- 📈 Dashboard for reviewing emotion summaries, session history, and risk alerts  
- 📤 Exportable reports for clinical tracking

---

## 🧠 Model Used

We use the Hugging Face model [`j-hartmann/emotion-english-distilroberta-base`](https://huggingface.co/j-hartmann/emotion-english-distilroberta-base), a lightweight DistilRoBERTa model fine-tuned for emotion detection in English.

- Understands 7–8 common human emotions (joy, sadness, anger, fear, etc.)  
- Optimized for short texts like therapy notes and journal entries  
- Fast and lightweight — ideal for integration into Streamlit

---

## 🗂️ Project Structure

```
therapy-session-analyzer/
├── app.py               # Main application entry point
├── database.db          # SQLite database for users, sessions, and emotions
├── requirements.txt     # Python dependencies
├── setup.py             # Installation script and project metadata
├── assets/
│   └── style.css        # Custom styling for Streamlit UI
├── components/
│   ├── dashboard.py     # Therapist dashboard and emotional trends
│   ├── patientview.py   # View emotion analysis for selected patient
│   └── exports.py       # Export patient data and reports
└── utils/
    ├── database.py      # Handles database operations (CRUD)
    └── auth.py          # Manages user login, signup, and logout
```

---

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/therapy-session-analyzer.git
cd therapy-session-analyzer
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Launch the App

```bash
streamlit run app.py
```

---

## 💬 Sample Use Case

**Input:**  
`I’m tired of pretending I’m okay. I feel so alone even when I’m surrounded.`

**Output:**  
- **Sadness:** 0.78  
- **Loneliness:** 0.69  
- **Hope:** 0.12

👉 The system extracts emotion scores from raw text and visualizes emotional states over time — helping therapists track their patients' well-being.

---

## 🔒 Therapist Features

- ✅ Login and manage sessions securely  
- 📝 Enter or import session text  
- 📊 View emotional trends and summaries  
- ⚠️ Get alerts on emotion spikes  
- 📥 Export reports for offline use

---

## 🛣️ Future Roadmap

- 🔊 Real-time voice-to-text analysis  
- 🌐 Multilingual support (using mBERT)  
- 🧠 Patient-side journaling assistant  
- ☁️ Full web deployment for clinics

---

## 👩‍💻 Built With

- **Frontend:** Streamlit + Custom CSS  
- **Backend:** Python, SQLite  
- **NLP Models:** Transformers (RoBERTa), BART, TextBlob, BERTopic  
- **Visualization:** Matplotlib, Streamlit charts

---

## 🙏 Acknowledgments

- [Hugging Face Transformers](https://huggingface.co/models)  
- [Streamlit](https://streamlit.io)  
- [j-hartmann/emotion-english-distilroberta-base](https://huggingface.co/j-hartmann/emotion-english-distilroberta-base)
