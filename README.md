# 🤝 Personalized Networking Assistant

An AI-powered networking assistant that helps users prepare for professional events by identifying event themes and generating relevant conversation starters.

## ✨ Features

- **User Profile:** Enter your name, profession, skills, interests, and bio.
- **Event Theme Analysis:** Identify the central theme of an event using AI.
- **AI Conversation Starters:** Generate professional networking conversation starters.
- **Conversation History:** Access previously generated conversations.
- **Feedback System:** Rate generated conversations and submit comments.
- **Fact Checker:** Submit topics for verification and view results.

## 🧰 Tech Stack

| Layer | Technologies |
|---|---|
| Frontend | Python, Streamlit |
| Backend | Python, FastAPI, Uvicorn |
| AI / NLP | Hugging Face Transformers, PyTorch |
| Data Processing | NumPy, Pandas |
| HTTP Communication | Requests |

## 📁 Project Structure

```text
Personalized-Networking-Assistant/
├── README.md
└── Personalized-Networking-Assistant-main/
    ├── Demo video/
    ├── Documents/
    ├── ER Daigram.png
    └── Project code/
        └── Personalized-Networking-Assistant/
            ├── ai_models/
            │   ├── conversation_generator.py
            │   ├── fact_checker.py
            │   └── theme_extractor.py
            ├── backend/
            │   ├── app.py
            │   ├── models.py
            │   ├── routes.py
            │   └── utils.py
            ├── frontend/
            │   └── streamlit_app.py
            ├── tests/
            └── requirements.txt
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/gowthusaidatta/Personalized-Networking-Assistant.git

cd Personalized-Networking-Assistant
```

### 2. Navigate to the application directory

```bash
cd "Personalized-Networking-Assistant-main/Project code/Personalized-Networking-Assistant"
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```cmd
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Start the FastAPI backend

```bash
uvicorn backend.app:app --reload
```

Backend URL: http://127.0.0.1:8000

API Documentation: http://127.0.0.1:8000/docs

### 6. Start the Streamlit frontend

Open another terminal, activate the virtual environment, navigate to the application directory, and execute:

```bash
streamlit run frontend/streamlit_app.py
```

Frontend URL: http://localhost:8501

**Important:** Start the FastAPI backend before launching the frontend.

## 🔌 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/` | Welcome message |
| GET | `/health` | Backend health status |
| GET | `/hello` | Check API routes |
| POST | `/user` | Create user profile |
| GET | `/users` | Retrieve users |
| POST | `/analyze` | Analyze event theme |
| POST | `/generate` | Generate conversation starters |
| GET | `/fact-check/{topic}` | Verify a topic |
| GET | `/history` | Retrieve conversation history |
| POST | `/feedback` | Submit feedback |
| GET | `/feedback` | Retrieve feedback history |

## 🔄 Application Workflow

1. Enter your professional profile.
2. Provide event title and description.
3. Analyze the event to identify its theme.
4. Generate personalized networking conversation starters.
5. Review the generated suggestions.
6. Submit feedback and ratings.
7. Access conversation and feedback history.

## 📸 Project Resources

- [Source Code](https://github.com/gowthusaidatta/Personalized-Networking-Assistant/tree/main/Personalized-Networking-Assistant-main/Project%20code)
- [Project Documents](https://github.com/gowthusaidatta/Personalized-Networking-Assistant/tree/main/Personalized-Networking-Assistant-main/Documents)
- [Demo Videos](https://github.com/gowthusaidatta/Personalized-Networking-Assistant/tree/main/Personalized-Networking-Assistant-main/Demo%20video)
- [ER Diagram](https://github.com/gowthusaidatta/Personalized-Networking-Assistant/blob/main/Personalized-Networking-Assistant-main/ER%20Daigram.png)

## 🚀 Future Improvements

- Database integration for persistent storage.
- User authentication and profile management.
- Customizable conversation styles.
- Improved error handling.
- Cloud deployment and scalability.

## 👨‍💻 Author

**Datta (Gowthu Sai Datta)**

GitHub: [@gowthusaidatta](https://github.com/gowthusaidatta)

## 📄 License

No license has been specified yet. Add a license before permitting reuse or distribution.
