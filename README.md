
# Generalized Conversational AI Assistant ⚡

This project is a **conversational AI assistant** designed to extract and provide answers from documents using advanced AI and NLP technologies. It can be customized for various use cases, including mining, legal, educational, healthcare, and more.

## Features
- 📖 **Document Processing**: Loads and processes PDF files.
- 🤖 **Conversational AI**: Utilizes OpenAI GPT models to deliver context-aware responses.
- 🔍 **Semantic Search**: Implements ChromaDB for fast and accurate information retrieval.
- 🌐 **Streamlit Frontend**: A user-friendly web interface for queries.

## General Use Cases
- Industry-specific advisors (e.g., mining, legal, healthcare).
- Educational content exploration.
- Document summarization and Q&A.
- Enterprise knowledge base assistants.

## Customizable Parts
1. **Document Loader**:
   - Replace the PDF file path or modify the loader to accept user-uploaded files.
   - Update the `process_file` method in `mini.py` to support other document formats like `.docx` or `.txt`.

2. **Domain-Specific Data**:
   - Customize the content and type of documents used (e.g., regulations, manuals, academic papers).
   - Modify the ChromaDB collection name to reflect the intended domain.

3. **API Key**:
   - Replace the placeholder `OPENAI_API_KEY_srijan` with your own OpenAI API key in the `api_key.py` file.

4. **Frontend Text**:
   - Update the Streamlit UI elements (titles, descriptions, etc.) to align with the chosen use case.
   - Modify lines such as `st.title(" ⚒️🌏⛏️ MiningMentor 👷‍♀️ _v1")` in `mini.py`.

5. **Query Processing**:
   - Adjust the `build_chain` method to change retrieval settings like the number of documents (`k` parameter).

6. **Output Handling**:
   - Customize how the results are displayed to the user in Streamlit, including formatting and additional insights.

## Prerequisites
- Python 3.8+
- OpenAI API Key
- Libraries:
  - `streamlit`
  - `langchain`
  - `chromadb`
  - `PyPDFLoader`
  - `openai`
  - `fitz`

## Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/conversational-ai.git
   cd conversational-ai
