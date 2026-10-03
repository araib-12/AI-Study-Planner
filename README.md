# AI Study Planner

Turn a learning goal into a structured plan, with explanations, leveled questions, and instant feedback, in one focused workspace.

## Overview

AI Study Planner is a Streamlit application that uses the free Google Gemini API to help you study with purpose. Describe what you want to learn, optionally attach reference material, and get an organized plan: topics broken down, explanations at the right level, and practice questions from easy to hard. Answer in the app, check your work against model feedback, and review mistakes and tips. It is useful for exam preparation or for building a new skill.

## Features

- **Structured study plans:** clear milestones and pacing based on your goal and time available
- **Topic breakdown:** subtopics and hierarchy so you know what to tackle next
- **Explanations:** content tuned to beginner, intermediate, or advanced level
- **Question sets:** easy, medium, and hard questions tied to the plan
- **Interactive answering:** submit answers and see verdicts with explanations and reference solutions
- **Modern UI:** tabbed workspace, light and dark themes, and local plan history
- **Optional PDF context** and SQLite storage keep plans grounded and saved

## Demo flow

1. Enter your study goal, level, and time. Optionally upload a PDF.
2. Generate the study plan and browse the Plan, Topics, and Learn tabs.
3. In Questions, write your answers and click Check answers.
4. Open Feedback for detailed results, and review Mistakes and Tips.
5. Use the sidebar to reopen saved plans and track checkpoints.

## Tech stack

| Part | Choice |
|------|--------|
| Language | Python |
| AI model | Google Gemini API (free tier) |
| Interface | Streamlit |

Supporting libraries: pypdf (PDF text extraction) and SQLite (local storage). The model is configurable in `config.py`.

## How to run

1. Install dependencies:
```
   pip install -r requirements.txt
```
2. Get a free API key at aistudio.google.com and set it (never commit real keys):
```
   export GEMINI_API_KEY="your_free_key"
```
3. Start the app:
```
   streamlit run app.py
```

## Author

Created by **Araib**, Civil Engineer.

Verify critical facts against your course materials when it matters.
