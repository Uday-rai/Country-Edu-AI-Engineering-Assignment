# AI Engineer project 

Two FastAPI services covering resume screening and a customer support knowledge base assistant.

## Structure

```
Uday/
├── Question_1_Resume_Screening_System/
│   ├── app/                  — FastAPI application
│   ├── sample_data/          — sample resumes and job descriptions
│   ├── tests/                — pytest test suite
│   ├── requirements.txt
│   ├── Dockerfile
│   ├── docker-compose.yml
│   └── README.md
└── Question_2_Customer_Support_AI_Assistant/
    ├── app/                  — FastAPI application
    ├── sample_data/          — FAQ and demo questions
    ├── tests/                — pytest test suite
    ├── requirements.txt
    ├── Dockerfile
    ├── docker-compose.yml
    └── README.md
```

## Quick start

Both services default to SQLite — no database setup or Docker required.

**Question 1 — Resume Screening:**

```bash
cd Question_1_Resume_Screening_System
pip install -r requirements.txt
uvicorn app.main:app --host 127.0.0.1 --port 8000
```

Open http://127.0.0.1:8000/dashboard/?v=3

**Question 2 — Customer Support Assistant:**

```bash
cd Question_2_Customer_Support_AI_Assistant
pip install -r requirements.txt
uvicorn app.main:app --host 127.0.0.1 --port 8010
```

Open http://127.0.0.1:8010/assistant

## Using Docker (optional — switches to PostgreSQL)

```bash
cd Question_1_Resume_Screening_System
docker-compose up --build
```

```bash
cd Question_2_Customer_Support_AI_Assistant
docker-compose up --build
```
