# LLM-AS-JUDGE

## Overview

LLM-AS-JUDGE is a Generative AI evaluation project that uses Large Language Models (LLMs) to generate responses and evaluate them automatically. The project helps in comparing, validating, and scoring AI-generated outputs using another LLM as a judge.

This project demonstrates:

* Dataset generation
* LLM-based response generation
* Automated evaluation using a judge model
* Modular Python project structure

---

# Features

* Generate golden evaluation datasets
* Generate answers using an LLM
* Evaluate generated responses automatically
* Modular and reusable Python scripts
* Virtual environment support using `uv`
* Easy execution using Python scripts

---

# Technologies Used

* Python 3.11
* Groq API
* Pandas
* NumPy
* Pydantic
* Rich
* Python-dotenv
* HTTPX

---

# Project Structure

```text
LLM-AS-JUDGE/
│
├── src/
│   ├── main.py
│   ├── evaluator.py
│   ├── generator_llm.py
│   ├── judge_llm.py
│   └── generate_dataset.py
│
├── requirements.txt
├── .env
└── README.md
```

---

# Installation

## 1. Clone the Repository

```bash
git clone <repository-url>
cd LLM-AS-JUDGE
```

---

## 2. Create Virtual Environment

```bash
uv venv
```

Activate the environment:

### Windows

```bash
.venv\Scripts\activate
```

---

## 3. Install Dependencies

```bash
uv pip install -r requirements.txt
```

---

# Environment Variables

Create a `.env` file in the root directory.

Example:

```env
GROQ_API_KEY=your_api_key_here
```

---

# Running the Project

## Generate Dataset

```bash
python src/generate_dataset.py
```

---

## Run Generator LLM

```bash
python src/generator_llm.py
```

---

## Run Judge LLM

```bash
python src/judge_llm.py
```

---

## Run Complete Evaluation

```bash
python src/main.py
```

---

# Workflow

1. Generate golden dataset
2. Generate responses using LLM
3. Judge model evaluates generated responses
4. Results are compared and scored

---

# Common Errors and Solutions

## ModuleNotFoundError: No module named 'evaluator'

Reason:

* File name mismatch
* Incorrect import statement

Solution:

* Ensure the file is named `evaluator.py`
* Verify import statement:

```python
from evaluator import run_evaluation
```

---

## File Not Found Error

Reason:

* Running Python command from wrong directory

Solution:

```bash
python src/main.py
```

---

# Future Improvements

* Add Streamlit frontend
* Add FastAPI backend
* Support multiple LLM providers
* Add evaluation dashboards
* Add score visualization graphs

---

# Author

Aniket Sawant

---

# License

This project is developed for educational and research purposes.
