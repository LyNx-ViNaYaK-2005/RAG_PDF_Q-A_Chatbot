# RAG PDF Q&A Chatbot

This project is a **Retrieval-Augmented Generation (RAG) chatbot** that answers questions based on the content of a PDF document. It uses **SentenceTransformers** for semantic search and **Google's Gemma LLM** for answer generation.

---
## Features

* **Extracts and chunks text** from PDF files
* **Embeds chunks** for semantic retrieval
* **Retrieves relevant context** for user queries
* **Generates answers** using a large language model (LLM)
* **Verifies factual alignment** between answer and context
* **Interactive command-line chat interface**

---
## Requirements

* **Python 3.8+**
* See `requirements.txt` for all dependencies

---
## Setup

1.  **Clone or download this repository.**
2.  **Install dependencies:**
    ```sh
    pip install -r requirements.txt
    ```
3.  **(Optional) Login to Hugging Face for model access:**
    ```sh
    huggingface-cli login
    ```
4.  **Run the notebook or script:**
    * Open `RAG_QA_Chatbot (1).ipynb` in Jupyter Notebook or VS Code.
    * Follow the prompts to load your PDF and start chatting.

---
## Usage

* Enter the path to your PDF file when prompted.
* Ask questions about the PDF content.
* **Use commands:**
    * `help` — Show available commands
    * `clear` — Clear conversation history
    * `info` — Show PDF and embedding info
    * `show context` — Display retrieved context for last question
    * `quit` or `exit` — Exit the chatbot

---
## Notes

* For best performance, use a machine with a **CUDA-capable GPU**.
* The chatbot uses the `all-mpnet-base-v2` embedding model and `google/gemma-2b-it` LLM.
* Fact verification is based on cosine similarity and is a heuristic.

---
## License

For academic and personal use only. See model licenses for details.
