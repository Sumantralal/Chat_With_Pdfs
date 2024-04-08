# Chat with PDFs 📚

## Introduction
The Chat with PDFs is a Python application that allows you to chat with multiple PDF documents. You can ask questions about the PDFs using natural language, and the application will provide relevant responses based on the content of the documents. This app utilizes a large language model to generate accurate answers to your queries. Please note that the app will only respond to questions related to the loaded PDFs and also give other general answers like LLM’s. Ex- ChatGPT 3.5, ChatGPT 4.0, Google’s Gemini and Claude.ai.

## Project Flow
The application follows these steps to provide responses to your questions:

1. **PDF Loading**: The app reads multiple PDF documents and extracts their text content.
2. **Text Chunking**: The extracted text is divided into smaller chunks that can be processed effectively.
3. **Language Model**: The application utilizes a language model(OpenAI Embedding Model APIs) to generate vector representations (embeddings) of the text chunks.
4. **Similarity Matching**: When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.
5. **Response Generation**: The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.

## Tools Used
- **Front-End**: Streamlit, an open-source Python framework.
- **Backend**: Python (3.12.2)
- **Framework Used**: LangChain (0.1.0), Streamlit (1.32.0)
- **Libraries**: PyPDF2 (3.1.0)
- **Vector Database**: ChromaDB
- **API’s**: OpenAI
- **Embedding Model**: OpenAI Embedding Model

## Installation
```bash
pip install streamlit PyPDF2 langchain python-dotenv openai


Run:
streamlit run app.py

How to use the app:
Step 1: Upload the pdfs through Browse files options.
Step 2: Click on Process button.
Step 3: Type your query you want to ask from the pdfs that you have
uploaded.
Step 4: And here you go, you can chat with the pdfs through this app.
