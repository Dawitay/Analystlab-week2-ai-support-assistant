# AI Customer Support Assistant — Week 2 (AnalystLab Africa Internship)

## Overview
Week 2 submission for the **Generative AI Internship Programme** at AnalystLab Africa. This project builds a functional AI-powered customer support assistant for a fictional client, **ABC Communications Ltd**, a telecom provider based in Addis Ababa, Ethiopia — extending the design work from Week 1 into a working application.

## What It Does
- Accepts a customer's support question as input
- Validates input (rejects empty, too-short, or excessively long text)
- Grounds every response in a local knowledge base of ABC's real plans, pricing, and troubleshooting steps (RAG-style)
- Sends the grounded prompt to Google's Gemini API (free tier)
- Displays the AI-generated response
- Escalates billing disputes and complaints to a human agent instead of resolving them itself
- Handles API errors (e.g. temporary outages) gracefully without crashing

## Tech Stack
- Python
- Google Gemini API (`google-genai`) — free tier, no credit card required
- Google Colab (notebook-based execution)

## Files in This Repository

| File | Description |
|---|---|
| `ABC_Support_Assistant_Colab_Gemini_FREE.ipynb` | Main application (Colab notebook, source code) |
| `requirements.txt` | Python dependencies |
| `Problem_Definition_Report.docx` | Business problem, target users, proposed solution, benefits, challenges |
| `Prompt_Evaluation_Report.docx` | 5 test prompts with purpose, AI response, evaluation, and suggested improvements |
| `Reflection_Report.docx` | Lessons learned, challenges, and future enhancements |
| `screenshots/` | Application screenshots showing user input, AI responses, and test scenarios |

## Setup Instructions
1. Open [Google Colab](https://colab.research.google.com/) and upload `ABC_Support_Assistant_Colab_Gemini_FREE.ipynb`
2. Get a free API key at [aistudio.google.com/apikey](https://aistudio.google.com/apikey) (no credit card required)
3. Run the notebook cells in order (Shift+Enter). When prompted, paste your API key.
4. Use Step 6 to ask a single question, Step 7 for a continuous chat loop, or Step 8 to run the 5 required test prompts automatically.

## Key Techniques Applied
- Context grounding (RAG-style) using a local knowledge base
- Role and guardrail prompting (escalation rules, anti-hallucination instructions)
- Input validation and graceful error handling
- Prompt-based tone control for frustrated/emotional customer scenarios

## About
Submitted as part of the AnalystLab Africa Generative AI Internship Programme, Week 2.

`#AnalystLabAfrica`
