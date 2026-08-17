
# Medical Chatbot (RAG-Based)

An intelligent Medical Chatbot built using a Retrieval-Augmented Generation (RAG) architecture. This application allows users to ask medical-related queries and get accurate, context-aware responses based on a provided medical knowledge base (PDF). 

The backend orchestrates the workflow using LangChain, stores and retrieves embeddings using Pinecone, and serves the user interface through a Flask web application.

## 🛠️ Tech Stack
*   **Language:** Python
*   **Orchestration:** LangChain
*   **Vector Database:** Pinecone
*   **Web Framework:** Flask
*   **Frontend:** HTML/CSS (via Flask Templates)

## 📁 Project Structure
*   `app.py`: The main Flask application script that runs the web server and handles routing.
*   `store_index.py`: A utility script used to process the raw PDF data, generate embeddings, and push them to the Pinecone vector database.
*   `data/`: Directory containing the source knowledge base (`Medical_book.pdf`).
*   `research/`: Contains Jupyter notebooks (`trials.ipynb`) for experimenting with data extraction, embeddings, and LangChain configurations.
*   `src/`: Contains the core modularized Python code for the chatbot logic.
*   `templates/` & `static/`: Holds the HTML, CSS, and JS files for the chatbot's web interface.
*   `requirements.txt`: Lists all Python dependencies required to run the project.
*   `.env`: Stores sensitive environment variables like API keys (not tracked by Git).

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone [https://github.com/Aishikmax/Medical-chatbot-_RAG-_based-.git](https://github.com/Aishikmax/Medical-chatbot-_RAG-_based-.git)
cd Medical-chatbot-_RAG-_based-
## 📊 Pipeline Evaluation (RAGAS)
To ensure the medical answers are accurate and mitigate LLM hallucinations, the RAG pipeline was evaluated using the **RAGAS** framework.
* **Answer Relevancy:** 86.2% (High precision in addressing user queries)
* **Faithfulness:** 50.0% (Highlighting areas for future strict-prompting improvements to enforce context-grounding)
* **Context Precision:** 50.0% (Vector search accuracy metric)
