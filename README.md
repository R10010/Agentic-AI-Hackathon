# ▲ PulseAI 
**Submission for Problem Statement: API Failure Detection & Debugging Agent**

> **PulseAI** is an intelligent observability agent that detects silent API failures, groups anomalies, and generates automated fix scripts before users even notice downtime.

## The Problem
Engineering teams struggle to detect silent API failures. Traditional monitoring tools throw thousands of raw logs at developers, leading to high Mean Time To Resolution (MTTR).

## Our Solution
PulseAI acts as an AI SRE (Site Reliability Engineer). It ingests telemetry data, parses the noise using LLMs, and outputs a clean incident report complete with **auto-generated bash scripts** to fix the infrastructure.

## Features 
- **AI Integration:** Uses Google Gemini 1.5 Flash to parse cryptic logs into plain English.
- **Smart Clustering:** Groups recurring failures to prevent alert fatigue.
- **Real-World Usability:** Generates runnable `.sh` fix scripts to instantly remediate server crashes.
- **UI/UX:** Built with a premium, Vercel/Linear-inspired dark mode interface.
- **Zero-Downtime Fallback:** Includes a local heuristic NLP engine that takes over if the API fails.

## Tech Stack
- **Frontend:** Vanilla JS, HTML5, CSS3 
- **Backend:** Python, Flask
- **AI:** Google Generative AI SDK

## How to Run Locally
1. Clone repo: `git clone [YOUR_REPO_LINK]`
2. Install dependencies: `pip install -r requirements.txt`
3. Add API Key: Create a `.env` file and add `GEMINI_API_KEY=your_key`
4. Run the app: `python app.py`
5. Open `http://localhost:5000`