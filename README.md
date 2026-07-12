# 🤖 Single Agent Pipeline using Conditional Routing

## 📌 Overview

This project demonstrates a simple **Single Agent Pipeline** built using Python. The agent intelligently routes user queries to different tools based on their intent using **conditional routing**.

The project was developed as part of the **Week 8 Assignment** on Agent Systems.

---

## 🚀 Features

- ✅ Calculator Tool
- ✅ Keyword Extraction Tool
- ✅ Conditional Query Routing
- ✅ Structured JSON Responses
- ✅ Input Validation
- ✅ Error Handling
- ✅ Automated Validation Tests
- ✅ Interactive Command-Line Interface

---

## 🛠️ Technologies Used

- Python 3
- Google Colab / Jupyter Notebook
- JSON
- Regular Expressions (`re`)

---

## 📂 Project Structure

```
.
├── CEI week_8_assignment
└── Short Quiz and small agent pipeline project.ipynb
```

---

## ⚙️ How It Works

The agent receives a user query and determines which tool should process it.

### Routing Logic

```
User Query
     │
     ▼
Input Validation
     │
     ▼
Contains "calculate"?
     │
 ┌───┴────┐
 │        │
Yes       No
 │        │
 ▼        ▼
Calculator Tool

          Contains "keywords"?
               │
          ┌────┴────┐
          │         │
         Yes        No
          │         │
          ▼         ▼
Keyword Tool   General Response
```

---

## 🧰 Available Tools

### 1. Calculator Tool

Evaluates mathematical expressions.

Example:

```
calculate 25 + 15
```

Output

```json
{
    "type": "calculation",
    "result": 40
}
```

---

### 2. Keyword Extraction Tool

Extracts important keywords by removing common stop words.

Example

```
keywords Artificial Intelligence is transforming education
```

Output

```json
{
    "type": "keywords",
    "result": [
        "artificial",
        "intelligence",
        "transforming",
        "education"
    ]
}
```

---

### 3. General Response

Handles all other queries.

Example

```
Hello Agent
```

Output

```json
{
    "type": "general",
    "result": "You said: Hello Agent"
}
```

---

## ▶️ Running the Project

1. Clone the repository

```bash
git clone https://github.com/your-username/your-repository.git
```

2. Open the notebook in Google Colab or Jupyter Notebook.

3. Run all cells.

4. Use the interactive agent at the end of the notebook.

5. Type **exit** to stop the program.

---

## 🧪 Sample Queries

Calculator

```
calculate 50 + 25
```

Keyword Extraction

```
keywords Machine Learning is changing healthcare
```

General Query

```
Hello
```

Exit

```
exit
```

---

## 📋 Assignment Objectives

- Build a rule-based single-agent system
- Implement conditional routing
- Integrate multiple tools
- Produce structured JSON outputs
- Handle invalid inputs gracefully
- Demonstrate validation through automated tests

---

## 📚 Learning Outcomes

Through this project, the following concepts were explored:

- Single-Agent Systems
- Agent Pipelines
- Conditional Routing
- Tool Integration
- JSON Response Formatting
- Error Handling
- Input Validation
- Interactive Agent Design

---

## 👨‍💻 Author

**Name:** Gagan Singh

---

## 📄 License

This project is intended for educational purposes only.
