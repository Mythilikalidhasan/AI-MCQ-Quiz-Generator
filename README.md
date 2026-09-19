# AI-MCQ-Quiz-Generator

An AI-powered Multiple Choice Question (MCQ) Quiz Generator built using **Python, Streamlit, and Hugging Face**.

The application allows users to enter a topic and automatically generates MCQ questions using an AI model. Users can select their answers and submit the quiz to see their score.

## Features

* Generate MCQs based on any topic
* Choose the number of questions
* AI-generated questions using Hugging Face
* Multiple-choice options for each question
* Automatic answer checking
* Displays the final score
* Simple and user-friendly Streamlit interface

## Technologies Used

* **Python** – Application development
* **Streamlit** – Web application interface
* **Hugging Face** – AI model for generating MCQs
* **VS Code** – Development environment

## Project Structure

```text
mcq_quiz_app/
│
├── app.py
├── requirements.txt
├── .gitignore
└── .streamlit/
    └── secrets.toml
```

## How It Works

1. Enter a topic, such as `Python`, `Java`, or `DBMS`.
2. Select the number of questions.
3. Click **Generate Quiz**.
4. The Hugging Face AI model generates the MCQs.
5. Select an answer for each question.
6. Click **Submit Quiz**.
7. The application calculates and displays your score.

## Installation

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
```

Move into the project folder:

```bash
cd mcq_quiz_app
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the virtual environment on Windows:

```powershell
venv\Scripts\activate
```

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

## Hugging Face API Token

Create a Hugging Face access token and store it securely in:

```text
.streamlit/secrets.toml
```

Add:

```toml
HF_TOKEN = "your_huggingface_token"
```

Do not upload `secrets.toml` to GitHub.

The `.gitignore` file should contain:

```text
.streamlit/secrets.toml
venv/
__pycache__/
```

## Running the Application

Run the following command in the VS Code terminal:

```powershell
python -m streamlit run app.py
```

The application will open in your browser.

Usually, Streamlit runs at:

```text
http://localhost:8501
```

## Example

### Input

```text
Topic: Python
Number of Questions: 5
```

### Output

The application generates questions such as:

```text
Which keyword is used to define a function in Python?

A. function
B. def
C. define
D. fun
```
<img width="802" height="865" alt="image" src="https://github.com/user-attachments/assets/d055b21c-5288-4058-8e8e-733059a1e960" />

After answering all questions, the application displays the final score.

## Future Improvements

* Add difficulty levels
* Add explanations for correct answers
* Add a quiz timer
* Add different categories
* Add score history
* Improve the user interface
* Add a leaderboard
* Deploy the application online

## Author

**Mythili K**

B.Sc. Computer Science with Artificial Intelligence
