# Langchain-Chat-with-search-from-Wikipedia-Arxiv-Duckduck

This repository contains a Streamlit application demonstrating a LangChain agent powered by Groq's fast LLM, capable of performing web searches, retrieving information from Arxiv, and querying Wikipedia.

## Overview

This application allows users to interact with a chatbot that can:

* **Search the web:** Using DuckDuckGo for general information retrieval.
* **Access research papers:** Querying Arxiv for academic publications.
* **Retrieve Wikipedia articles:** Obtaining quick facts and summaries.
* **Provide real-time feedback:** Utilizing `StreamlitCallbackHandler` to display the agent's thought process.
* **Leverage Groq's Llama3-8b-8192:** For fast and efficient language model processing.
* **Maintain chat history:** For seamless conversational interactions.

## Features

* **Interactive Chat Interface:** Built with Streamlit for a user-friendly experience.
* **Multi-Tool Integration:** Combines web search, Arxiv, and Wikipedia for comprehensive information retrieval.
* **Real-time Agent Feedback:** Shows the agent's reasoning and actions during the search process.
* **Groq LLM Powered:** Utilizes Groq for rapid response times.
* **Easy Setup:** Simple configuration with API key input.

## Getting Started

### Prerequisites

* Python 3.7+
* Groq API Key (You can obtain one from the Groq website)

### Installation

1.  Clone the repository

2.  Create a virtual environment (recommended):

3.  Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

4.  Run the Streamlit application:

    ```bash
    streamlit run app.py
    ```

5.  Enter your Groq API key in the sidebar when prompted.

### Environment Variables

* Ensure you have a `requirements.txt` file listing all the libraries your app requires.

### Usage

1.  Open the Streamlit application in your web browser.
2.  Enter your Groq API key in the sidebar.
3.  Type your query in the chat input and press Enter.
4.  Observe the agent's thought process and the final response.

## Code Explanation

* `app.py`: Contains the Streamlit application code, including agent initialization and interaction logic.
* The application uses LangChain to orchestrate the agent and integrate the various tools.
* Groq's `ChatGroq` LLM is used for language processing.
* `StreamlitCallbackHandler` provides real-time feedback on the agent's actions.

## Dependencies

* `streamlit`
* `langchain`
* `langchain_groq`
* `langchain_community`
* `python-dotenv`
