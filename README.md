# RAG Chatbot with Pinecone

This project implements a Retrieval-Augmented Generation (RAG) chatbot using Pinecone for vector search and OpenAI for language generation. It is designed to efficiently ingest, store, and query large datasets for conversational AI applications.

## Features
- Ingests data in parallel batches into Pinecone
- Uses OpenAI models for generating responses
- Environment variable management with dotenv
- Modular and extensible code structure

## Setup

1. **Clone the repository**
   ```sh
   git clone https://github.com/kinola-IQ/Rag-chatbot-with-pinecone.git
   cd Rag-chatbot-with-pinecone
   ```

2. **Install dependencies**
   ```sh
   pip install -r requirements.txt
   ```

3. **Configure environment variables**
   - Create a `.env` file in the project root:
     ```env
     pinecone_api_key=YOUR_PINECONE_API_KEY
     openai_api_key=YOUR_OPENAI_API_KEY
     ```

4. **Prepare your data**
   - Place your CSV file in the project directory and update the `filepath` variable in `script.ipynb`.

## Usage

- Open `script.ipynb` in Jupyter or VS Code.
- Run the cells to:
  - Load libraries and environment
  - Ingest data into Pinecone
  - Query the index and generate responses

## File Structure
- `script.ipynb`: Main notebook for data ingestion and chatbot logic
- `requirements.txt`: Python dependencies
- `.env`: Environment variables (not tracked in git)

## Example
```python
from pinecone import Pinecone, ServerlessSpec
from openai import OpenAI
# ...
```

## License
MIT

## Author
kinola-IQ
