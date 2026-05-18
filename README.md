# Prompt-Engineering
# Generative AI-Powered Email Management System
**Johns Hopkins University — AI Course Midterm Project**

<img width="700" height="500" alt="Screenshot 2026-05-17 at 10 38 55 PM" src="https://github.com/user-attachments/assets/a9eef0b6-fd20-4211-9d9f-e93889e51611" />

---

## Project Overview
This project builds an AI-powered email management system that helps a business leader manage their inbox efficiently using the **Yesterbox productivity approach** — focusing on yesterday's emails to prioritize actions for today. The system uses prompt engineering on a large language model to automate email categorization, summarization, and response drafting.

---

## Dataset
- **File:** `Alex_emails_march_04.csv`
- **Description:** A dataset of business emails received by a Senior Manager at a mid-sized IT company
- **Size:** 60 emails across multiple recipients
- **Fields:** `email_id`, `date_received`, `sender`, `subject`, `body`, `main_recipient`

---

## Project Structure

### Data Preprocessing
- Load email dataset
- Apply Yesterbox filtering — emails from March 3rd, 2025 only
- Filter emails for the target recipient

---

### Task 1 — Email Summarization

#### Categorization
Emails are classified into one of six predefined categories:
1. Urgent & High-Priority Emails
2. Deadline-Driven Emails
3. Routine Updates & Check-ins
4. Non-Urgent Informational Emails
5. Personal & Social Emails
6. Spam/Unimportant Emails

#### 1A — Executive Dashboard
Generates a top-level summary of the inbox including:
- Total email count
- Breakdown by category
- AI conclusion highlighting critical vs non-critical emails

#### 1B — Urgent Emails Summary
Summarizes all Urgent & High-Priority emails with:
- Subject, Sender, Received date
- One-sentence summary
- Specific next step for each email

#### 1C — Deadline-Driven Emails Summary
Summarizes all Deadline-Driven emails with:
- Full email details
- Next steps focused on meeting deadlines
- Final count and summary of actionable items

---

### Task 2 — AI-Drafted Responses
Generates professional first response drafts for all critical emails (Urgent + Deadline-Driven) including:
- Acknowledgement of the sender's request
- Key points addressed
- Clear next step
- Polite and professional tone

---

### Task 3 — LLM-as-a-Judge Evaluation
Evaluates the quality of AI-drafted responses across three dimensions:
- **Relevance** — Does the response address the email content?
- **Clarity** — Is the response clear and easy to understand?
- **Actionability** — Does the response provide clear next steps?

Results are stored in a structured DataFrame with scores and justifications.

---

## Key Concepts Applied
- Prompt Engineering (Zero-Shot, One-Shot, Role Prompting)
- Yesterbox Productivity Approach
- LLM-as-a-Judge Evaluation Framework
- Structured Output Formatting

---

## Requirements
- Python 3.x
- Jupyter Notebook
- pandas
- tqdm
- LLM API access (course-provided)

---

## How to Run
1. Upload `Alex_emails_march_04.csv` to your notebook environment
2. Open `JHU_AGAI_W9_Mid_Term_Project_Solution_Notebook_12th_Feb.ipynb`
3. Run all cells in order from top to bottom
4. Outputs will be displayed inline in the notebook

---

## Results Summary
- Relevance: 5/5 across all evaluated responses
- Clarity: 5/5 across all evaluated responses
- Actionability: Mostly 4/5 — minor improvements needed around specific timelines and follow-up steps

---

## Author
**JHU AI Course — Midterm Project**


<img width="700" height="600" alt="Screenshot 2026-05-17 at 10 39 22 PM" src="https://github.com/user-attachments/assets/0aed9194-3c72-4791-a1e6-7a670add8c80" />

