# TeXtract

**TeXtract** is a tool designed for math students and researchers to extract and summarize key formulas, theorems, and proofs from digital documents (PDF/EPUB). It uses advanced NLP (Natural Language Processing) and LLMs (Large Language Models) to identify and format relevant mathematical content into LaTeX, providing users with a clean, professional PDF output.

## Features

- Upload PDF/EPUB files and extract mathematical content.
- Summarize important formulas, theorems, and proofs directly from the text.
- Generate LaTeX-formatted documents and compile them into PDFs.
- Uses state-of-the-art NLP and LLMs to ensure accuracy in extraction and summarization.
- Supports customization of output (e.g., headings, level of detail).

## Tech Stack

- **Frontend**: Vue.js
- **Backend**: Node.js (for handling uploads and communication with the Python service)
- **Processing**: Python (for NLP, LLM-based summarization, and LaTeX generation)
  - **Libraries**: PyMuPDF, EbookLib, spaCy, Hugging Face Transformers, PyLaTeX
- **LaTeX Compilation**: pdflatex

## How It Works

1. **File Upload**: Users upload a PDF or EPUB file containing mathematical content.
2. **Content Extraction**: The backend parses the document, and Python's NLP/LLM-based system extracts key formulas, theorems, and proofs.
3. **LaTeX Generation**: The extracted content is formatted into LaTeX.
4. **PDF Compilation**: The LaTeX is compiled into a final PDF document, ready for download.
5. **Output**: Users receive a clean, concise PDF summarizing the most important information from their uploaded document.

## Setup and Installation

### Prerequisites

- **Node.js** and **npm**
- **Python 3.x** and **pip**
- **LaTeX** (ensure `pdflatex` is installed for PDF compilation)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/TeXtract.git

2. Install the required dependencies:
   - **Node.js (Backend)**:
     ```bash
     cd TeXtract/backend
     npm install
     ```
   - **Python (Processing)**:
     ```bash
     cd TeXtract/python
     pip install -r requirements.txt
     ```

3. Run the application:
   - **Node.js Backend**:
     ```bash
     npm run dev
     ```
   - **Python Service**:
     ```bash
     python app.py
     ```

4. Access the frontend via the localhost URL (e.g., `http://localhost:3000`).
