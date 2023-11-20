# Agri-mche Chatbot

## Introduction

This repository contains the code for the Agri-mche chatbot, utilizing language models for question answering and a vector store for similarity search. The chatbot uses LangChain for natural language processing tasks.

## Prerequisites

Before running the code, make sure you have the following dependencies installed:

- Python (version 3.6 or higher)
- [FAISS](https://github.com/facebookresearch/faiss) for efficient similarity search
- [LangChain](https://github.com/NCATS-Tangerine/langchain) for natural language processing
- [dotenv](https://github.com/theskumar/python-dotenv) for loading environment variables

## Setup

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/agri-mche-chatbot.git
    cd agri-mche-chatbot
    ```

2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Create a `.env` file:**
    Create a `.env` file in the project root and populate it with the necessary environment variables:

    ```env
    LLAMA_EMBEDDINGS_MODEL=/path/to/llama/model
    MODEL_TYPE=openai  # or gpt4all depending on your configuration
    MODEL_PATH=/path/to/gpt4all/model  # or specify the OpenAI API key if using OpenAI
    MODEL_N_CTX= # Add the value for MODEL_N_CTX
    OPEN_AI_API_KEY= # Add your OpenAI API key
    ```

4. **Load the FAISS index:**
    - Uncomment the relevant lines in the script to create and save the index initially.
    - Run the script once to create and save the index.
    - Comment out the index creation part and uncomment the line to load the index from the file for subsequent runs.

## Usage

Run the chatbot script:

```bash
python chatbot.py
