# Intelligent Document Question Answering System using RAG

## About the Project

This project allows users to upload a PDF document and ask questions about its content. It uses Retrieval-Augmented Generation (RAG) to find relevant information from the PDF and generate answers using a locally running Llama 3 model.

## Technologies Used

- Python
- Streamlit
- PyPDF2
- Sentence Transformers
- FAISS
- NumPy
- Ollama
- Llama 3

## Features

- Upload PDF documents.
- Extract text from PDF files.
- Split text into smaller chunks.
- Convert text into embeddings.
- Store embeddings using FAISS.
- Search for relevant information based on a question.
- Generate answers using Llama 3.
- Display retrieved context and answers in a web interface.

## How the Project Works

1. Upload a PDF document.
2. Extract text from the PDF.
3. Split the text into smaller chunks.
4. Generate embeddings using Sentence Transformers.
5. Store the embeddings in FAISS.
6. Enter a question about the PDF.
7. Retrieve the most relevant text chunks.
8. Send the question and context to Llama 3.
9. Display the generated answer.

## Installation and Setup

### 1. Clone the Repository

Open Command Prompt or PowerShell and run:

```bash
git clone https://github.com/Kavitaa2003/Intelligent_Document_Question_Answering_System.git
```

Go to the project folder:

```bash
cd Intelligent_Document_Question_Answering_System
```

### 2. Create a Virtual Environment

```cmd
python -m venv .venv
```

Activate it in Command Prompt:

```cmd
.venv\Scripts\activate
```

### 3. Install Python Dependencies

Create a file named `requirements.txt` containing:

```text
streamlit
PyPDF2
faiss-cpu
numpy
requests
sentence-transformers
```

Install the packages:

```cmd
pip install -r requirements.txt
```

### 4. Install Ollama

Download and install Ollama from:

https://ollama.com/download

Download the Llama 3 model:

```cmd
ollama pull llama3
```

Make sure Ollama is running on your computer.

### 5. Run the Project

If your main Python file is named `app.py`, run:

```cmd
streamlit run app.py
```

Open the local URL displayed in the terminal. It is usually:

http://localhost:8501

## How to Use

1. Open the application in your browser.
2. Upload a PDF document.
3. Wait for the document to be processed.
4. Enter a question related to the PDF.
5. View the retrieved context and generated answer.

## Important Notes

- Python and Ollama must be installed.
- The Llama 3 model must be downloaded before asking questions.
- The first run may take time because the embedding model needs to download.
- Scanned PDFs may not work correctly because OCR is not implemented.
- The application uses a local Ollama API at `http://localhost:11434/api/generate`.

## Author

**Kavita Anil Shewale**

## GitHub Repository

https://github.com/Kavitaa2003/Intelligent_Document_Question_Answering_System
