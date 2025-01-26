# StackUp Assistant: AI-Powered FAQ Chatbot

## Overview
The **StackUp Assistant** is a conversational AI chatbot designed to answer user queries based on a predefined dataset of FAQs. It leverages advanced natural language processing (NLP) techniques and a large language model (LLM) to provide accurate and context-aware responses. The chatbot is built using the **LangChain** framework, **HuggingFace Embeddings**, and **Google's Gemini** model, ensuring robust performance and scalability.

This project was developed as part of my learning journey on **StackUp**, a learn-and-earn platform that empowers individuals to build real-world projects while gaining valuable skills.

## Features
- **Natural Language Understanding**: The chatbot uses HuggingFace embeddings and LangChain's retrieval mechanisms to understand and process user queries.
- **Dynamic Response Generation**: Powered by Google's Gemini LLM, the chatbot generates human-like responses tailored to the user's input.
- **Interactive GUI**: The chatbot features a user-friendly interface built with **Taipy**, allowing users to interact seamlessly.
- **Customizable Dataset**: The chatbot can be trained on any dataset of FAQs stored in `.txt` files, making it adaptable to various domains.

## Preview
Here’s a screenshot of the chatbot in action:

![Chatbot Screenshot](https://github.com/Reedwarn/TaipyTrail/blob/8a9ded14ee35fc425f49b41b45a9042253b6b2ac/data/preview.png)

## Technologies Used
- **Python**: The core programming language used for development.
- **LangChain**: Framework for building LLM-powered applications.
- **HuggingFace Embeddings**: For generating vector representations of text.
- **Google Generative AI (Gemini)**: LLM for generating responses.
- **Taipy**: For building the interactive graphical user interface (GUI).
- **Pandas**: For data manipulation (if needed).
- **Dotenv**: For managing environment variables.

## How It Works
1. **Data Loading**: The chatbot loads FAQs from `.txt` files stored in the `./data` directory.
2. **Document Indexing**: The FAQs are split into chunks, embedded using HuggingFace, and indexed for efficient retrieval.
3. **Query Processing**: When a user submits a query, the chatbot retrieves the most relevant information from the indexed dataset.
4. **Response Generation**: The retrieved information is passed to the Gemini LLM, which generates a natural language response.
5. **User Interaction**: The chatbot displays the response in an interactive GUI, allowing for continuous conversation.
