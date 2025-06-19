# 🧠 AI-Powered Company Brochure Generator

## 📄 Overview

This project is an intelligent brochure-generation tool powered by **Large Language Models (LLMs)** that automatically scrapes company websites and generates structured, markdown-based brochures. These brochures are tailored for prospective **clients, investors, and recruits**.

Given a **company name** and its **website URL**, the system:
- Scrapes the website’s content and important links (like About, Careers, etc.)
- Parses and processes the data using LLMs
- Generates a professional, human-readable marketing brochure

This showcases an **Agentic AI design pattern**, where multiple intelligent components work together to analyze, reason, and generate business content.

---

## 🚀 Key Features

- 🌐 **Web Scraping**: Extracts meaningful content and metadata from any company's website
- 🧠 **LLM Integration**: Uses `GPT-4o-mini` or `LLaMA 3.2` locally via OpenAI-compatible API
- 📄 **Structured Output**: Returns a well-formatted marketing brochure in Markdown format
- 🔗 **Link Intelligence**: Filters and enriches site links using one-shot prompting
- 🧩 **Agentic Pattern**: Makes multiple intelligent calls across stages — gathering, reasoning, and composing

---

## 🛠️ Tech Stack

| Component          | Description                                     |
|-------------------|-------------------------------------------------|
| **Python**         | Core programming language                       |
| **OpenAI SDK**     | Interface for local LLMs (e.g., LLaMA3.2 via Ollama) |
| **BeautifulSoup**  | For HTML parsing and scraping                   |
| **Requests**       | For fetching raw website HTML                   |
| **Markdown Display** | To render outputs inside Jupyter Notebook     |
| **Dotenv**         | Secure API key handling                         |

---

## 💡 How It Works

1. **Input**: Provide a company name and URL (e.g., `"Amazon"`, `"https://amazon.com"`).
2. **Scraping**: The `Website` class fetches and cleans textual content from the landing page and relevant subpages (About, Careers, etc.).
3. **Link Filtering**: A prompt-based LLM call determines which links are brochure-worthy (excluding privacy, TOS, etc.).
4. **Brochure Assembly**:
    - All content is structured and sent as a prompt to the LLM
    - The model responds with a detailed brochure including sections like:
      - Company Mission
      - Company Culture
      - Customer Base
      - Careers & Hiring
      - Contact Information
5. **Display**: The brochure is printed to screen or streamed interactively with typewriter-like animation using `display()`.

---

## 📦 Example Use Case: Amazon

Input: `"Amazon", "https://amazon.com"`

The system outputs a marketing brochure including:
- Mission: Earth’s most customer-centric company
- Culture: Innovation, inclusion, leadership principles
- Careers: Roles like Software Engineer, Logistics Professional, Customer Support
- Sustainability efforts
- Contact details and hiring page

---

## 🎯 Why This Project Matters

Marketing brochures are a staple for businesses but creating them manually is:
- Time-consuming
- Repetitive
- Prone to outdated info

With this tool:
✅ Startups can instantly generate polished company overviews  
✅ Enterprises can automate internal or public marketing docs  
✅ Recruiters can send dynamic company briefs to job applicants  
✅ Investors get concise insights about a firm without digging

 
