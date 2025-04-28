
# 🧠 AI Agent: Text Classifier, Entity Extractor, and Summarizer

This project implements a simple yet powerful **AI agent** that processes any input text through a three-step pipeline:
1. **Classification** — Categorizes the text (News, Blog, Research, Tech, Other).
2. **Entity Extraction** — Extracts named entities (Person, Organization, Location).
3. **Summarization** — Generates a short one-sentence summary.

The agent is built using **LangGraph**, **LangChain**, and **OpenAI's GPT models**.

Ref: https://medium.com/data-science-collective/the-complete-guide-to-building-your-first-ai-agent-its-easier-than-you-think-c87f376c84b2
---

## 🚀 Features

- **Multi-step Agent Workflow**: Orchestrated using a state graph.
- **Zero-shot Classification**: Classifies texts into meaningful categories.
- **Named Entity Recognition (NER)**: Extracts key people, organizations, and locations.
- **Summarization**: Condenses the input into a single, concise sentence.
- **Modular Code Structure**: Easy to extend with more nodes or custom logic.

---

## 🛠️ Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Create and activate a virtual environment** (recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**:
   - Create a `.env` file in the project root.
   - Add your OpenAI API key:
     ```
     OPENAI_API_KEY=your-openai-api-key
     ```

---

## 📄 Usage

Run the main script:
```bash
python main.py
```

Example output:
```
Classification: Tech

Entities: ['Anthropic']

Summary: Anthropic's MCP enables easy API interaction across systems.
```

---

## 🧩 Project Structure

```
.
├── main.py         # Main script containing the agent logic
├── .env            # Environment variables (not uploaded to GitHub)
├── requirements.txt# Python dependencies
└── README.md       # Project documentation
```

---

## 📚 Requirements

- Python 3.8+
- [langgraph](https://pypi.org/project/langgraph/)
- [langchain](https://pypi.org/project/langchain/)
- [python-dotenv](https://pypi.org/project/python-dotenv/)
- [openai](https://pypi.org/project/openai/)

Install all at once:
```bash
pip install langgraph langchain openai python-dotenv
```

---

## 🔥 Future Improvements

- Add error handling (e.g., for missing fields).
- Support additional entity types (Dates, Events, etc.).
- Introduce branching paths based on classification.
- Replace OpenAI with local models (optional).
- Deploy as a web app using FastAPI or Streamlit.

---

## 📜 License

This project is open-sourced under the [MIT License](LICENSE).

---

## ✨ Acknowledgements

- [LangChain](https://langchain.dev/)
- [LangGraph](https://langgraph.dev/)
- [OpenAI API](https://platform.openai.com/)
