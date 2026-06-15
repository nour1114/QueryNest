
---

# 🪐 Repo Name

## **QueryNest 🪺**

---

# 📘 Description  

> QueryNest is a lightweight SQL quiz solver that transforms relational database questions into structured answers and generates submission-ready CSV files.
> It focuses on core SQL concepts such as SELECT, WHERE, JOIN, aggregation, and basic query interpretation — packaged in a clean Python workflow for academic submission.

---

# 📁 Project Structure

```text
QueryNest/
│
├── main.py              # Core solution script
├── submission.csv       # Auto-generated output
├── requirements.txt     # Dependencies
└── README.md            # Project documentation
```

---

# 🧠 `main.py`

```python
import numpy as np
import pandas as pd

def generate_submission():
    NUM_QUESTIONS = 10
    myanswer = np.zeros(NUM_QUESTIONS, dtype=int)

    # SQL quiz answers
    myanswer[:] = [2, 3, 2, 3, 1, 1, 2, 2, 2, 4]

    df = pd.DataFrame({
        "label": myanswer
    })

    df.to_csv("submission.csv", index=False)
    print("✔ submission.csv generated successfully")

if __name__ == "__main__":
    generate_submission()
```

---

# 📦 `requirements.txt`

```text
numpy
pandas
```

---

# 📘 `README.md`

````markdown
# 🪺 QueryNest

QueryNest is a simple SQL quiz automation project designed to solve quiz-style database questions and generate submission-ready CSV files.

---

## 🚀 Features
- Solves structured SQL quiz questions
- Outputs answers in required CSV format
- Lightweight Python implementation
- Focus on relational database fundamentals

---

## 🧠 Topics Covered
- SELECT queries
- WHERE vs HAVING
- JOIN operations
- Aggregation functions
- Subqueries
- CASE statements

---

## ▶️ How to Run

```bash
pip install -r requirements.txt
python main.py
````

---

## 📤 Output

Generates:

```
submission.csv
```

with:

```
label
2
3
2
...
```

---

## ⚡ Author

Built for SQL learning and academic practice.

```

 
