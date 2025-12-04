# Study RAG: Flask + Gemini File Search App

A simple, clean **study assistant web app** built with **Flask** and **Google Gemini**.  
You can upload your study notes (PDF, DOC, TXT, etc.) and then ask questions based on those notes.  
The app sends your questions to Gemini and shows the answer in a nicely formatted way. Self-hosted the app using **Pinggy.io**.
Check:https://pinggy.io/blog/how_to_use_file_search_tool_in_gemini_api_for_easy_rag_integration/

## ✨ Features

- 📝 **Upload notes** (e.g., `.txt`, `.pdf`, `.doc`)
- 🔎 **Ask questions** about your uploaded notes
- 🧠 Uses **Google Gemini** (`gemini-2.0-flash-lite-preview`) for answering
- 📚 **File Search integration** via Gemini File Search Store
- ✅ Success message when a file is uploaded and indexed
- ⚠ Friendly message when API quota (429 RESOURCE_EXHAUSTED) is hit
- 🧾 Answer shown in **clean paragraphs** with basic formatting (Markdown → HTML)
- 🎨 Simple & clean UI built with HTML + inline CSS

![Application_demo1](https://github.com/Bidisha314/Study-APP/blob/main/Application_demo1.gif)
![Application_demo2](https://github.com/Bidisha314/Study-APP/blob/main/Application_demo2.gif)

## 🧱 Tech Stack

- **Backend:** Python, Flask
- **LLM / RAG:** Google Gemini via `google-genai` SDK
- **Frontend:** HTML (Jinja templates), minimal inline CSS
- **Template Engine:** Jinja2 (Flask default)
- **Tunneling Tool:** Pinggy (https://pinggy.io/)
- **Formatting:** `markdown` Python library to render AI output nicely


## 📂 Project Structure

Example structure:

```bash
study-rag/
├─ app.py
├─ requirements.txt
├─ templates/
│  └─ index.html
└─ static/          # (optional, for images/icons if you add them later)


