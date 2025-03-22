# Explainable_Chatbot

This project is a conversational AI chatbot built with LangChain, Hugging Face, and Pinecone. It uses a transformer model to generate responses, stores conversation history in a Pinecone vector database for context, and includes a feature to delete stale history to keep memory fresh. The chatbot is designed to explain text input in a creative and detailed way, making it a fun tool for learning and exploration.

## Features
- **Conversational AI**: Powered by the `Qwen/QwQ-32B` model from Hugging Face.
- **Persistent Memory**: Stores chat history in Pinecone with embeddings from `all-MiniLM-L6-v2`.
- **Stale History Cleanup**: Deletes older messages while keeping the most recent ones (default: last 5).
- **Interactive CLI**: Simple command-line interface with options to chat, clear stale history, or exit.

## Tech Stack
- **Python**: Core programming language.
- **LangChain**: For building the conversation chain and prompt templating.
- **HuggingFaceEndpoint**: Integrates the Qwen model for text generation.
- **Sentence Transformers**: Generates embeddings for storing conversations.
- **Pinecone**: Vector database for managing chat history.

## Prerequisites
- Python 3.8+
- A Hugging Face account and API token ([get one here](https://huggingface.co/settings/tokens)).
- A Pinecone account and API key ([sign up here](https://www.pinecone.io/)).

## Setup
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/chatbot-with-pinecone-memory.git
   cd chatbot-with-pinecone-memory
