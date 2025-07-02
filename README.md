# 💻 MCP Sentiment Analysis

Welcome to **MCP Sentiment**, a simple yet powerful web app that analyzes the sentiment of any text using 💬 **Natural Language Processing (NLP)** powered by 🐍 Python, 🤗 Hugging Face Spaces, and ⚙️ Gradio.

---

## 🚀 What is this project?

MCP Sentiment is a lightweight text sentiment analyzer that lets users input any sentence or paragraph and receive:

- 📊 **Polarity**: How positive or negative the sentiment is (from -1 to +1)
- 🧠 **Subjectivity**: How opinionated the sentence is (from 0 to 1)
- 📌 **Assessment**: A simple label: `Positive`, `Negative`, or `Neutral`

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| 🐍 Python | Core programming |
| 🧠 [TextBlob](https://textblob.readthedocs.io/en/dev/) | NLP & Sentiment Analysis |
| 🎨 [Gradio](https://gradio.app/) | Frontend UI |
| ☁️ [Hugging Face Spaces](https://huggingface.co/spaces) | Hosting & Deployment |
| 🔧 Git | Version control |
| 🔍 Powershell + CMD | Local development |

---

## 📦 Features

- ✅ Simple textbox input
- ✅ Clean sentiment output in JSON format
- ✅ Live deployment on Hugging Face
- ✅ Uses `textblob.sentiment` under the hood
- ✅ MCP-compatible server support

---

## 📚 How it works

1. You type any sentence in the textbox.
2. The backend uses **TextBlob** to calculate:
   - Polarity (`-1.0` = very negative, `1.0` = very positive)
   - Subjectivity (`0.0` = very objective, `1.0` = very subjective)
3. The result is shown instantly with a sentiment **assessment**.

---

## ⚒️ Development Journey (with Debugging)

> ✅ Every bug was a lesson:

- 🐛 Python not detected → Solved by using `py` launcher on Windows
- 🐘 Accidentally added `venv/` → Caused large file push errors
- 📦 Fixed `.gitignore` to skip tracking `venv/`
- 🔁 Git history issues → Cleaned by removing `.git` and reinitializing
- 🛑 Push errors (`fetch first`) → Solved with `--force` push
- 📄 Typo in `requirement.txt` → Renamed to correct `requirements.txt`
- ✅ Final clean push to Hugging Face → LIVE!

---

## 🔗 Live Demo

👉 Try it out here:  
[https://huggingface.co/spaces/csaisurya/mcp-sentiment](https://huggingface.co/spaces/csaisurya/mcp-sentiment)

---

## 🧠 Try sample inputs:

- `"I absolutely love this app!"` → Positive
- `"This is the worst experience ever."` → Negative
- `"It's okay, not great but not bad."` → Neutral

---

## 🧰 How to run locally

```bash
git clone https://github.com/cherypallysaisurya/mcp-sentiment-analysis.git
cd mcp-sentiment
python -m venv venv
venv\Scripts\activate   # For Windows
pip install -r requirements.txt
python app.py
