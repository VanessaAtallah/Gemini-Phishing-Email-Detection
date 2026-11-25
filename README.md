# Gemini Phishing Email Detection

An AI-powered phishing email detection system that uses **Google Gemini 2.5 Flash** and **LangChain** to analyze email content, identify suspicious URLs, and classify emails as phishing or legitimate.

## Features

- **Email Parsing:** Extracts the sender, subject, email body, and URLs from `.eml` files.
- **Feature Extraction:** Detects suspicious indicators such as urgent language, credential requests, suspicious domains, and typosquatting patterns.
- **URL Analysis:** Uses Gemini to assess URLs and identify potential security risks.
- **AI Classification:** Classifies emails as phishing or legitimate and assigns a risk score.
- **Explainable Results:** Provides detected signals, explanations, and user recommendations.
- **Sender-Based Memory:** Maintains conversation history for each sender to consider previous email activity during analysis.

## Technologies Used

- Python
- Google Gemini 2.5 Flash
- LangChain
- Google Colab

## How It Works

1. Upload an `.eml` email file.
2. Extract email information and identify URLs.
3. Analyze email features and suspicious indicators.
4. Assess URLs using Gemini.
5. Classify the email and calculate its risk score.
6. Generate an explanation and recommendation.
7. Store the analysis in sender-based memory for future reference.

## Risk-Based Actions

The system assigns an action based on the calculated risk score:

- **Allow:** Risk score ≤ 50%
- **Warn:** Risk score between 51% and 80%
- **Block:** Risk score > 80%

## Setup and Usage

1. Open the `Gemini_Phishing_Email_Detection.ipynb` notebook.
2. Install the required dependencies.
3. Provide your Google Gemini API key when prompted.
4. Run the notebook cells.
5. Upload an `.eml` file to analyze the email.
6. Review the classification, risk score, detected signals, and recommendation.

## Note

This project is designed as an email security analysis tool. Its classifications and recommendations should be treated as indicators rather than a guarantee that an email is safe or malicious.
