Bostonia Assistant 🤖💬
Chat with a Boston City Bot - LangChain Chatbot with Streamlit GUI
Welcome to the GitHub repository for the Boston City LangChain Chatbot with Streamlit GUI! This project is a comprehensive guide to building a chatbot capable of interacting with websites, extracting information, and communicating in a user-friendly manner. It leverages the power of LangChain 0.1.0 and integrates it with a Streamlit GUI for an enhanced user experience.

Features
Website Interaction: The chatbot uses the latest version of LangChain to interact with and extract information from wikipedia website of Boston City.
Large Language Model Integration: Compatibility with models like GPT-4, Mistral, Llama2, and ollama. In this code we have used GPT-4.
Streamlit GUI: A clean and intuitive user interface built with Streamlit, making it accessible for users with varying levels of technical expertise.
Python-based: Entirely coded in Python.
Brief explanation of how RAG works
A RAG bot is short for Retrieval-Augmented Generation. This means that we are going to "augment" the knowledge of our LLM with new information that we are going to pass in our prompt. We first vectorize all the text that we want to use as "augmented knowledge" and then look through the vectorized text to find the most similar text to our prompt. We then pass this text to our LLM as a prefix.

Here is a diagram that shows the process:

RAG Diagram

Steps to run
Install the required packages:

pip install -r requirements.txt
Create your own .env file with the following variables:

OPENAI_API_KEY=[your-openai-api-key]
Usage
To run the Streamlit app:

streamlit run app.py