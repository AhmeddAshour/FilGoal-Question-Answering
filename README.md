# FilGoal Question Answering System Using LangChain

## Project Overview
This project aims to develop an **Arabic Question Answering (QA) System** that answers queries related to football (soccer) using web-scraped articles. The system processes text using **Natural Language Processing (NLP)** techniques, including **AraBERT**, a model fine-tuned for Arabic text. The goal is to retrieve the most relevant chunks of text from a large dataset of football-related articles and provide accurate answers to user queries.

This system is designed to handle questions in Arabic, making it highly suitable for Arabic-speaking users interested in football news, transfers, team stats, match results, and other football-related topics.

The primary objectives of this project include:

- Scraping football-related news articles.
- Processing the text to extract useful information.
- Using a **pre-trained Arabic language model** (AraBERT) for generating embeddings.
- Storing these embeddings in a **FAISS index** for efficient similarity-based retrieval.
- Answering user queries based on relevant information retrieved from the documents.

## Technologies Used
The project utilizes the following technologies and libraries:

- **BeautifulSoup4**: A Python library for parsing HTML and XML documents. It is used to scrape articles and data from the FilGoal website.
- **Requests**: A simple HTTP library for making requests to the website to retrieve HTML content.
- **Pandas**: A powerful data manipulation and analysis library for handling and processing the scraped data.
- **Transformers**: A library by Hugging Face for working with pre-trained NLP models, including **AraBERT**, specifically designed for Arabic text.
- **FAISS (Facebook AI Similarity Search)**: A library for efficient similarity search. It is used to store the embeddings and perform fast similarity-based retrieval.
- **LangChain**: A framework to simplify the development of applications using language models. Although the project doesn't directly use LangChain for processing, it is part of the workflow for managing document handling and splitting.
- **PyTorch**: A machine learning library used by **AraBERT** to generate embeddings for text.
