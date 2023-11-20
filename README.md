# Agri-mche Chatbot

## Introduction

This repository contains the code for the Agri-mche chatbot, a conversational agent that leverages natural language processing and similarity search for agricultural advice. The chatbot utilizes advanced language models and vector stores for efficient question answering.

## Technology Stack

- **Programming Language:**
  - Python

- **Libraries and Frameworks:**
  - [LangChain](https://github.com/NCATS-Tangerine/langchain): A library for natural language processing tasks.
  - [FAISS](https://github.com/facebookresearch/faiss): A library for efficient similarity search.

- **Machine Learning Models:**
  - [GPT-4](https://www.openai.com/): A powerful language model by OpenAI for natural language understanding and generation.
  - [LLAMA (Linguistic Learning with a Message-Adapting architecture)](https://llamallama.readthedocs.io/en/latest/): A library for embedding and similarity tasks.

- **Vector Store:**
  - [FAISS](https://github.com/facebookresearch/faiss): A library for similarity search and clustering of dense vectors.

- **Environment Management:**
  - [dotenv](https://github.com/theskumar/python-dotenv): A library for loading environment variables from a file.

- **Version Control:**
  - Git: Used for version control of the source code.

- **Documentation:**
  - Markdown: Used for writing documentation (e.g., README).

- **Other Tools:**
  - TextLoader: Part of LangChain, possibly used for loading text documents.
  - StreamingStdOutCallbackHandler: A callback handler for streaming standard output in LangChain.

- **APIs:**
  - OpenAI API: Used for inplace of  the GPT-4 language model if the `MODEL_TYPE`.

## Prerequisites

Before running the code, make sure you have the required dependencies installed. Check the [Setup](#setup) section for detailed instructions.

## Setup

Follow these steps to set up the project:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/AmosMaru/Mche-chatbot.git
    cd Mche-chatbot
    ```

2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Create a `.env` file:**
    Create a `.env` file in the project root and populate it with the necessary environment variables. Refer to [`.env.sample`](.env.sample) for an example.

4. **Load the FAISS index:**
    - Uncomment the relevant lines in the script to create and save the index initially.
    - Run the script once to create and save the index.
    - Comment out the index creation part and uncomment the line to load the index from the file for subsequent runs.

## Usage

Run the chatbot script:

```bash
python chatbot.py
