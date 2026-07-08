<div align="center">

# AI-Powered Lead Generation Agent

**Built and maintained by [Muhammad Muazzain](https://github.com/MuhammadMuazzain)**

A lead generation tool that scrapes fresh B2B contact data, then uses OpenAI to qualify, enrich, and suggest outreach strategies—all in a Streamlit UI.

<img src="https://img.shields.io/badge/python-3.9+-blue" /> <img src="https://img.shields.io/badge/OpenAI-API-blueviolet" /> <img src="https://img.shields.io/badge/Author-Muhammad%20Muazzain-success" />

</div>

---

## Author

| | |
|---|---|
| **Name** | Muhammad Muazzain |
| **GitHub** | [github.com/MuhammadMuazzain](https://github.com/MuhammadMuazzain) |
| **Repository** | [ai-lead-generator](https://github.com/MuhammadMuazzain/ai-lead-generator) |

---

## Features

- 🕵️‍♂️ **Automated Web Scraping:** Collect fresh leads from sources like LinkedIn via a scraping API.
- 📈 **AI-Powered Qualification:** Analyze, score, and enrich leads using OpenAI.
- 💡 **Natural Language Input:** Describe your ideal lead; the agent extracts structured filters and runs the workflow.
- 🤝 **Outreach Suggestions:** Personalized tips for email or LinkedIn engagement, tailored per lead.
- 🖥 **Interactive UI:** Manage the pipeline and settings from a Streamlit dashboard.

---

## Prerequisites

- Python 3.9+
- Scraping API token (Bright Data or compatible)
- [OpenAI API Key](https://platform.openai.com/api-keys)
- [Streamlit](https://streamlit.io/) installed
- (Optional) `python-dotenv` for API key management

---

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/MuhammadMuazzain/ai-lead-generator.git
   cd ai-lead-generator
   ```

2. **Create and activate a Python virtual environment**
   ```bash
   python -m venv venv
   # macOS/Linux: source venv/bin/activate
   # Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install streamlit openai requests python-dotenv brightdata
   ```

4. **Set API credentials**
   - Create a `.env` file:
     ```env
     OPENAI_API_KEY=your_openai_api_key_here
     BRIGHT_DATA_API_KEY=your_scraping_api_key_here
     ```
   - Or enter them directly in the Streamlit sidebar.

---

## Usage

1. **Launch the application**
   ```bash
   streamlit run app.py
   ```

2. **Open in your browser**
   - Visit `http://localhost:8501` (auto-opens)

3. **Describe your lead**
   - Enter a natural language query like:  
     `Find marketing managers in fintech companies in Kenya.`
   - Click **Generate Leads**.

4. **Review enriched results**
   - See fully scored, ranked, and enriched leads.
   - Each lead features an AI summary, relevance score, and outreach tip.

---

## How It Works

1. **Natural Language Query:** Type your requirements (role, industry, location, etc.).
2. **Filter Extraction:** OpenAI parses your query into structured API filters.
3. **Lead Data Collection:** The scraping API fetches targeted lead data.
4. **AI Enrichment:** Each lead is scored, summarized, and given engagement suggestions via OpenAI.
5. **Interactive Exploration:** Results appear in Streamlit with cards and scores.

---

## Output Features

- **AI-Scored Leads:** Ranking and insights without spreadsheets.
- **Relevance & Outreach Tips:** Why each lead matches and how to engage.
- **Customizable Workflow:** Adjust lead count, enrichment depth, or ICP prompt.
- **Debug Mode:** Trace decisions and API calls.

---

## Configuration

### .env file

```env
OPENAI_API_KEY=your_openai_api_key_here
BRIGHT_DATA_API_KEY=your_scraping_api_key_here
```

### Sidebar Settings

- **Scraping API Key:** Paste key (or use `.env`)
- **OpenAI API Key:** Paste key (or use `.env`)
- **Model Selector:** e.g., GPT-3.5, GPT-4o, etc.
- **Max Leads:** Number of leads to fetch (default: 10)

---

## Troubleshooting

- **No Leads Found**
  - Check API keys and dataset access
  - Relax search filters (role, location, etc.)
  - Use debug mode for detailed errors

- **Enrichment Fails**
  - Confirm your OpenAI API key is valid and not rate-limited
  - Check network connectivity

- **Scraping API Errors**
  - Ensure your token has the correct permissions
  - Review your provider’s API documentation

---

## License

This project is maintained by **Muhammad Muazzain** for educational and personal use.

---

## Links

- [Streamlit Documentation](https://docs.streamlit.io/)
- [OpenAI Platform Docs](https://platform.openai.com/docs)
- [Author on GitHub](https://github.com/MuhammadMuazzain)

---

**Ready to supercharge your sales prospecting? Clone this repo and turn lead search into qualified opportunities.**

---

**© 2026 Muhammad Muazzain · [ai-lead-generator](https://github.com/MuhammadMuazzain/ai-lead-generator)**
