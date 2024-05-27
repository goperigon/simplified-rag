# Simplified RAG

This repository contains a Python Jupyter Notebook that implements a simple **Retrieval-Augmented Generation (RAG)** pipeline using various state-of-the-art AI tools and APIs. This setup demonstrates how you can fetch the data from the web, use APIs to retrieve data, embed documents into a vector database, and create a chat-based language model to answer user queries with relevant information.

## Structure

The notebook is structured as follows:

1. **Environment Setup**:

   - Install necessary libraries and tools.

   - Run Playwright for the first time if required.

2. **Data Preparation**:

   - Scrape documents from the web.

   - Load documents from the Perigon API.

   - Split documents into chunks.

3. **Document Embedding**:

   - Embed documents into a vector database using `Qdrant`.

   - Retrieve documents based on similarity queries.

4. **Initialize Language Models**:

   - Set up various LLMs such as Ollama, Groq, and OpenAI ChatGPT.

5. **Testing Prompts**:

   - Query the models directly and via Retrieval-Augmented Generation (RAG).

## Setup

### Pre-requisites

- Python 3.7 or above

- Jupyter Notebook

### Installation

**Before Running the Notebook please make sure to set up environment variables:**

Create a `.env` file in the root directory of the project and add the following variables:

```sh
PERIGON_API_KEY=your_perigon_api_key
GROQ_API_KEY=your_groq_api_key
OPENAI_API_KEY=your_openai_api_key
```