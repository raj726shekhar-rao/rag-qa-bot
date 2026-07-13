# RAG Q&A Bot

Ask questions about any PDF document using AI.
Built with OpenAI embeddings, ChromaDB, and Streamlit.

## Demo
[Live demo link] | [Screenshot]

## How it works
1. Upload a PDF → text is chunked and embedded
2. Ask a question → top relevant chunks are retrieved
3. GPT-4o-mini answers using only those chunks as context

## Tech stack
- OpenAI text-embedding-3-small (embeddings)
- ChromaDB (vector store)
- LangChain (chunking)
- Streamlit (UI)

## Run locally
git clone git@github.com:yourusername/rag-qa-bot.git
cd rag-qa-bot
python -m venv venv && venv\Scripts\activate
pip install -r requirements.txt
streamlit run app.py

## Environment variables
Create a `.env` file with:
OPENAI_API_KEY=your-key-here
