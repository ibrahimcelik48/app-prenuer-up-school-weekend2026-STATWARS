# 🏀 NBA Quiz App - LLM-Optimized Development Plan

## 📌 Overview

This document is structured for **LLM-assisted development** (e.g., Cursor, Copilot, ChatGPT).
Each task is atomic, contains clear inputs/outputs, and can be executed independently.

---

## 🎯 MVP Goals

* Start an NBA quiz
* Answer multiple-choice questions
* Get a score at the end
* Basic UI + working API

---

## 🏗️ Architecture

```
nba-quiz-app/
│
├── backend/
│   ├── routes/
│   ├── controllers/
│   ├── services/
│   ├── models/
│   └── app.js
│
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── services/
│   └── App.jsx
│
└── plan.md
```

---

## ⚙️ GLOBAL RULES (FOR LLM)

* Always write modular, clean code
* Use clear naming conventions
* Do not hardcode values unless specified
* Return JSON responses from backend
* Handle errors explicitly

---

# 🚀 TASK BREAKDOWN (LLM EXECUTION READY)

## 🔹 TASK 1: Backend Initialization

### Prompt for LLM

```
Create a Node.js Express backend project with a basic server setup.
Include routing structure and middleware support.
```

### Expected Output

* Express server running on port 3000
* Folder structure created

### Acceptance Criteria

* Server starts without error
* GET / returns "API running"

---

## 🔹 TASK 2: Question Model

### Prompt

```
Create a Question model in JavaScript with fields: question, options (array), answer.
```

### Expected Output

```json
{
  "question": "string",
  "options": ["A","B","C","D"],
  "answer": "string"
}
```

### Acceptance Criteria

* Model is reusable
* Valid JSON structure

---

## 🔹 TASK 3: Quiz Routes

### Prompt

```
Create Express routes for quiz:
GET /quiz/start
POST /quiz/submit
```

### Expected Output

* Route files
* Controller integration

### Acceptance Criteria

* Endpoints return valid JSON

---

## 🔹 TASK 4: Quiz Logic Service

### Prompt

```
Implement a service that:
- Returns 5 quiz questions
- Validates answers
- Calculates score
```

### Expected Output

```json
{
  "score": 3,
  "total": 5
}
```

### Acceptance Criteria

* Correct scoring logic
* No crashes on invalid input

---

## 🔹 TASK 5: Frontend Initialization

### Prompt

```
Create a React app with routing.
Include pages: Home, Quiz, Result.
```

### Acceptance Criteria

* App runs
* Navigation works

---

## 🔹 TASK 6: Quiz UI

### Prompt

```
Build a quiz interface:
- Show question
- Show 4 options
- Next button
```

### Acceptance Criteria

* User can select answers
* Moves to next question

---

## 🔹 TASK 7: API Integration

### Prompt

```
Connect frontend to backend using fetch/axios.
```

### Acceptance Criteria

* Data loads from API
* No CORS issues

---

## 🔹 TASK 8: Result Page

### Prompt

```
Display quiz results after submission.
```

### Acceptance Criteria

* Score shown correctly

---

## 🔹 TASK 9: Error Handling

### Prompt

```
Add error handling for API and UI.
```

### Acceptance Criteria

* No crashes
* User sees meaningful messages

---

## 🔹 TASK 10 (OPTIONAL): LLM Question Generator

### Prompt

```
Use OpenAI API to generate NBA questions dynamically.
```

### Example Prompt

```
Generate 5 NBA quiz questions with 4 options and correct answers in JSON format.
```

### Acceptance Criteria

* Valid JSON response
* Questions usable in app

---

## 📊 SUCCESS CRITERIA

* Full quiz flow works
* Backend + frontend connected
* Clean, modular code

---

## 🧠 HOW TO USE THIS FILE WITH LLMs

1. Copy one TASK at a time
2. Paste into Cursor / ChatGPT
3. Generate code
4. Verify acceptance criteria
5. Move to next task

---

## 👨‍💻 Author

NBA Quiz App - LLM Optimized Plan
