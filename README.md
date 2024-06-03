# Chat_with_Multiple_PDF
Gen AI Project

This project allows users to upload multiple PDF files and ask questions based on the content of those PDFs. It leverages the power of Google Generative AI, LangChain, and FAISS to provide accurate answers from the provided documents.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Requirements](#requirements)
- [Contributing](#contributing)
- [License](#license)

## Features
- Upload multiple PDF files
- Extract text from PDF files
- Split text into manageable chunks
- Store text chunks in a vector store
- Ask questions and get answers based on the uploaded PDFs' content

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/Chat_with_Multiple_PDF.git
    cd Chat_with_Multiple_PDF
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up your Google API key:
    - Create a `.env` file in the project directory.
    - Add your Google API key to the `.env` file:
      ```
      GOOGLE_API_KEY=your_google_api_key
      ```

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. In the Streamlit interface:
    - Upload your PDF files using the file uploader in the sidebar.
    - Click on "Submit & Process" to process the PDFs.
    - Ask your questions in the main input box and get responses based on the content of the uploaded PDFs.

## Requirements

- Python 3.x
- streamlit
- google-generativeai
- python-dotenv
- langchain
- PyPDF2
- chromadb
- faiss-cpu
- langchain_google_genai
