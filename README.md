#  AI News Summarizer Agent (n8n + OpenRouter)

An automated AI workflow that fetches the latest AI news, summarizes it using a free LLM, and sends a daily email digest.

##  Features

* Fetches AI articles via RSS
* Summarizes content using OpenRouter (free LLM)
* Sends formatted email summaries
* Runs automatically every day at 8:00 AM

##  Architecture

Schedule Trigger → RSS Feed → Filter Latest Article → LLM (OpenRouter) → Email (Gmail)

##  Tech Stack

* n8n (workflow automation)
* OpenRouter (LLM API)
* Gmail API

##  Setup Instructions

1. Import `workflow.json` into n8n
2. Add your credentials:

   * OpenRouter API key
   * Gmail OAuth2
3. Update:

   * RSS feed URL
   * Recipient email
4. Activate the workflow

##  Example Output

* 5 bullet point summary
* Key insights from the article
* Link to full article

##  Future Improvements

* Filter only "AI agent" related news
* Summarize multiple articles into one digest
* Store summaries in a database (Notion/Airtable)
* Build a frontend dashboard

##  Author

Muhammad Faraz Malik
