# README: RAG Chatbot for Health Products

This repository contains a Retrieval-Augmented Generation (RAG) chatbot designed to provide information about the health benefits of various products based on a dataset. The chatbot leverages OpenAI embeddings, Qdrant for vector search, and Hugging Face's GPT-2 for response generation.

## Features
- **Query-based Information Retrieval**: Retrieves relevant information from a dataset based on user queries.
- **Qdrant Vector Search**: Efficient similarity-based search for context retrieval.
- **Hugging Face GPT-2**: Generates responses using a fine-tuned language model.
- **Environment Variable Management**: Securely handles API keys using a `.env` file.

## Prerequisites
- Python 3.8 or higher
- Kaggle Notebook or local Python environment

## Setup
### Clone the Repository
```bash
git clone https://github.com/yourusername/rag-chatbot.git
cd rag-chatbot
```

### Install Dependencies
Install the required Python packages:
```bash
pip install -r requirements.txt
```

### Prepare the Dataset
1. Ensure your dataset (`InfoHealthFood_20241225.xlsx`) is placed in the project directory.
2. The dataset should contain the following columns:
   - `許可證字號`: Product ID
   - `中文品名`: Product Name
   - `保健功效`: Health Benefits

### Configure Environment Variables
Create a `.env` file with the following content:
```
OPENAI_API_KEY=your_openai_api_key_here
```
Alternatively, provide the path to your `.env` file (e.g., `/kaggle/input/openai-env/.env`).

### Run the Chatbot
1. Launch the Python script:
   ```bash
   python rag_chatbot.py
   ```
2. Enter a query to interact with the chatbot. Type `exit` to quit.

### Notebook Version
If you prefer running the chatbot in a Jupyter notebook, the `rag-chatbot.ipynb` file is also included.

## Example Query
```text
Enter a product name to check its health benefits (or type 'exit' to quit):
什麼可以調血脂
Response:
  - e脂100膠囊 的保健功效是: 調節血脂
  - 健康調合油 的保健功效是: 調節血脂
  - 無加糖鮮豆漿 的保健功效是: 調節血脂功能
```

## Files
- `rag-chatbot.py`: Main script for the chatbot.
- `rag-chatbot.ipynb`: Jupyter notebook version of the chatbot.
- `requirements.txt`: List of dependencies.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments
- **OpenAI** for embeddings and GPT-2 model.
- **Qdrant** for vector search capabilities.
- **Hugging Face** for transformer models.

## Contact
For questions or issues, please contact [your_email@example.com].


