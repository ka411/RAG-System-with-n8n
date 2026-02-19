RAG System with n8n

This project implements a Retrieval-Augmented Generation (RAG) pipeline in n8n
.
It connects a chat interface with company/contract documents stored in Google Drive, allowing an AI agent to answer user queries using both memory and retrieved knowledge.


🚀 Features

Chatbot trigger: responds to chat messages.

AI Agent with memory: powered by gpt-4o-mini, keeps track of conversation context.

Document ingestion: downloads PDFs from Google Drive, extracts text, splits into chunks, and generates embeddings with OpenAI.

Vector Store: stores embeddings in memory for fast retrieval.

Knowledge retrieval: AI agent pulls relevant chunks from documents when answering questions.

RAG flow: user queries are enhanced with context before generating a response.

⚙️ Setup Instructions

Import RAG_System_5.json into your n8n instance.

Configure credentials for:

OpenAI API

Google Drive

Could you place relevant company/contract documents in Google Drive?

Trigger the workflow by sending a chat message.


🔮 Future Improvements

Persist vector store in a database (Pinecone, Weaviate, etc.) instead of in-memory.

Support multiple file formats (e.g., DOCX, XLSX).

Deploy chatbot to Slack, Teams, or a web interface.
