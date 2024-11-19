---

# NVIDIA NIM-Based Document QA Web Application

A state-of-the-art **Question-Answering (QA) web application** built using NVIDIA NIM inferencing and LangChain. This application provides interactive document-based question answering with highly accurate responses, powered by FAISS vector search and NVIDIA embeddings.

---

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Project Workflow](#project-workflow)
5. [Directory Structure](#directory-structure)
6. [Setup Instructions](#setup-instructions)
    - [Prerequisites](#prerequisites)
    - [Installation Steps](#installation-steps)
7. [How to Use](#how-to-use)
8. [Example Screenshot](#example-screenshot)
9. [Future Enhancements](#future-enhancements)
10. [Contributing](#contributing)
11. [License](#license)

---

## 1. Overview

This project is a **Streamlit-based web application** that allows users to upload documents, embed them using NVIDIA NIM's advanced LLMs, and ask context-based questions interactively. It employs cutting-edge machine learning and retrieval-augmented generation (RAG) techniques to provide precise answers while enabling similarity searches for related content.

### Core Objectives:
- Seamlessly process and embed large documents.
- Provide accurate answers to user queries based on document content.
- Support interactive and intuitive user experience through a simple UI.

---

## 2. Features

- **Document Embedding**:
  - Uses NVIDIA embeddings to convert document content into meaningful vectors.
- **Vector Database**:
  - Leverages FAISS for fast and efficient similarity searches.
- **Custom Prompting**:
  - Dynamically structures prompts using LangChain for accurate LLM responses.
- **Interactive QA**:
  - Allows users to input queries and receive answers in real time.
- **Document Similarity Search**:
  - Displays relevant chunks of content to enhance the user experience.
- **User-Friendly Interface**:
  - Built using Streamlit for an intuitive and clean design.

---

## 3. Technologies Used

- **[Streamlit](https://streamlit.io/)**: For building the web application UI.
- **[LangChain](https://www.langchain.com/)**: Framework for document processing and chaining.
- **[FAISS](https://github.com/facebookresearch/faiss)**: For efficient vector search and retrieval.
- **[NVIDIA NIM](https://developer.nvidia.com/)**: Powering inferencing with NVIDIA Llama3 70B model.
- **Python**: Backend logic for integrating all components.

---

## 4. Project Workflow

1. **Document Loading**:
   - Load documents from the specified directory (`iit_kgp_project`).
2. **Text Splitting**:
   - Break documents into manageable chunks for embedding.
3. **Embedding**:
   - Generate vector embeddings using NVIDIA NIM's embedding model.
4. **Vector Storage**:
   - Store embeddings in a FAISS vector database for similarity search.
5. **Query Processing**:
   - Retrieve relevant chunks and generate answers using NVIDIA Llama3.
6. **Similarity Search**:
   - Display related chunks for additional context.

---

## 5. Directory Structure

```plaintext
nvidia-nim-qa-webapp/
├── iit_kgp_project/           # Directory for storing PDF documents
├── app.py                     # Main Streamlit application script
├── requirements.txt           # List of dependencies
├── README.md                  # Documentation file
├── .env                       # Environment variables (e.g., NVIDIA API Key)
```

---

## 6. Setup Instructions

### 6.1 Prerequisites

- **Python 3.8 or above**.
- **NVIDIA API Key** for NIM inferencing.
- Basic knowledge of Streamlit for running the application.

### 6.2 Installation Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/nvidia-nim-qa-webapp.git
   cd nvidia-nim-qa-webapp
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure Environment**:
   - Create a `.env` file in the root directory and add your NVIDIA API Key:
     ```plaintext
     NVIDIA_API_KEY=your-nvidia-api-key
     ```

4. **Add Documents**:
   - Place your PDF files in the `iit_kgp_project` directory.

5. **Run the Application**:
   ```bash
   streamlit run app.py
   ```

---

## 7. How to Use

1. **Initialize Document Embedding**:
   - Click the **"Document Embedding"** button to process documents and build the FAISS vector database.

2. **Ask Questions**:
   - Enter your question in the text input box and click submit.
   - The application retrieves the most relevant document chunks and generates an accurate answer.

3. **Explore Similarity Search Results**:
   - Expand the **"Document Similarity Search"** section to view document chunks related to the query.

---

## 8. Future Enhancements

- **Add File Upload Support**:
  - Allow users to upload documents dynamically from the UI.
- **Support Additional Formats**:
  - Extend document processing to include Word documents, text files, etc.
- **Enhanced Retrieval**:
  - Use hybrid retrieval methods for better performance.
- **Performance Optimization**:
  - Improve response times by optimizing chunking and embedding workflows.

---

## 9 **Contributors**

- **Rishikesh**  
- LinkedIn: www.linkedin.com/in/rishikesh-a12090285
- Email: rishikesh23@kgpian.iitkgp.ac.in



## 10. License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute this software as per the license terms.

---
