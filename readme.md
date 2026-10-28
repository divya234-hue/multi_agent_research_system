# 🔬 ResearchMind — Multi-Agent AI Research System

An AI-powered research assistant that uses multiple specialized agents to search the web, extract relevant information, generate structured research reports, and critique the final output.

## 🚀 Overview

ResearchMind automates the research process through a multi-agent workflow. It combines web search, webpage content extraction, AI-generated report writing, and a critique stage to help users explore topics more efficiently.

## ✨ Features

- 🔎 **Web Search:** Finds relevant information using Tavily Search.
- 📄 **Webpage Extraction:** Extracts readable content from selected webpages.
- ✍️ **AI Report Generation:** Creates structured reports using GPT-4o-mini.
- 🧐 **AI Critic:** Reviews the generated report and provides a score, strengths, and areas for improvement.
- 🖥️ **Interactive Interface:** Streamlit-based research dashboard.
- 📥 **Report Export:** Download the generated research report in Markdown format.

## 🏗️ Architecture

ResearchMind follows a sequential research pipeline:

1. **Search Agent** — searches the web for relevant information.
2. **Reader Agent** — extracts detailed content from a selected webpage.
3. **Writer Chain** — generates a structured research report.
4. **Critic Chain** — evaluates the report and suggests improvements.
5. **Streamlit UI** — displays the research results and final report.

## 🛠️ Tech Stack

- **Programming Language:** Python
- **LLM:** OpenAI GPT-4o-mini
- **AI Framework:** LangChain
- **Web Search:** Tavily API
- **Web Scraping:** Requests, BeautifulSoup
- **Frontend:** Streamlit
- **Environment Management:** python-dotenv

## 📁 Project Structure

```text
ResearchMind/
│
├── agents.py          # Search and reader agents, writer and critic chains
├── app.py             # Streamlit web interface
├── pipeline.py        # Research pipeline orchestration
├── tools.py           # Web search and webpage scraping tools
├── requirements.txt   # Python dependencies
├── .gitignore         # Files excluded from Git
└── README.md          # Project documentation
```

**Note:** The `.env` file contains API keys and should remain private. It should never be committed to GitHub.

## 🔄 Workflow

```text
Research Topic
      ↓
Search Agent (Tavily)
      ↓
Reader Agent (Web Scraping)
      ↓
Writer Chain (GPT-4o-mini)
      ↓
Critic Chain (Report Evaluation)
      ↓
Final Research Report
      ↓
Streamlit Dashboard
```

## ⚠️ Current Limitations

- The pipeline scrapes one selected webpage for deeper research.
- Extracted webpage content is limited to 3,000 characters.
- The reader receives a truncated portion of the search results.
- The critic's score is AI-generated and is not independently verified.
- Search results and citations may require manual verification.

## 🔮 Future Improvements

- Parallel research agents for faster research
- Multi-source content extraction
- Citation verification and source reliability scoring
- Persistent research history
- Automated testing and deployment
- Improved error handling and source validation

## 👩‍💻 Author

**Divya Bharti**  
B.Tech — Artificial Intelligence & Data Science  
Poornima University, Jaipur

- **GitHub:** [@divya234-hue](https://github.com/divya234-hue)

---

⭐ If you find this project useful, consider giving it a star!