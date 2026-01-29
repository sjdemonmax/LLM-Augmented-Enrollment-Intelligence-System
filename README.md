# LLM-Augmented Enrollment Intelligence System

**Tech Stack:** Python, SQL, scikit-learn, OpenAI API  
**Focus:** GenAI + NLP + Applied ML for business decision automation

---

## Problem Statement
Educational platforms receive large volumes of **unstructured learner feedback** and behavioral data, making it difficult to:
- Understand sentiment and intent at scale
- Identify high-quality leads
- Personalize recommendations efficiently

Traditional analytics struggled with text-heavy signals and manual analysis.

---

## Solution Overview
Built a **production-style GenAI system** that combines:
- Classical ML models for prediction & ranking
- Prompt-engineered LLM workflows for NLP and insight generation

The system automates **sentiment analysis, lead scoring, and executive insight delivery**.

---

## System Architecture
Learner Data \(\rightarrow \) ETL/Engineering \(\rightarrow \) ML Models \(\rightarrow \) LLM Processing \(\rightarrow \) Structured Output \(\rightarrow \) Insights 


### Design Principles
- **ML models** → deterministic scoring & ranking  
- **LLMs** → unstructured text understanding & summarization  
- **Prompts treated as code** (versioned, tested, reusable)

---

## Key Features

### 1. LLM-Based Feedback Intelligence
- Sentiment classification
- Intent detection (pricing, pacing, difficulty, support)
- Urgency scoring for escalation

**Impact:**  
Reduced manual feedback review by **60%**

---

### 2. Enrollment Propensity & Lead Scoring (ML)
- Logistic regression & tree-based models  
- Features: engagement, academic history, behavioral signals  
- Evaluated using ROC-AUC & Precision-Recall  

**Impact:**  
Improved qualified lead conversion by **18–22%**

---

### 3. Prompt-Engineered Insight Generation
Used LLMs to automatically translate analytics into:
- Leadership summaries
- Risk & opportunity flags
- Actionable recommendations

---

## Sample Prompt (Structured Classification)

```text
System: You are an NLP analyst for an ed-tech platform.
User: Classify the feedback into {sentiment, intent, urgency}.
Return JSON only.

Feedback:
"The course is good but the pacing feels too fast before exams."
## Output
{
  "sentiment": "mixed",
  "intent": "curriculum pacing",
  "urgency": "medium"
}
---
