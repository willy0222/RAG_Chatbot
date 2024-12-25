# README: RAG Chatbot for Health Products

This repository contains a Retrieval-Augmented Generation (RAG) chatbot designed to provide information about the health benefits of various products based on a dataset. The chatbot leverages OpenAI embeddings, Qdrant for vector search, and Hugging Face's GPT-2 for response generation.

## Features
- **Query-based Information Retrieval**: Retrieves relevant information from a dataset based on user queries.
- **Qdrant Vector Search**: Efficient similarity-based search for context retrieval.
- **Hugging Face GPT-2**: Generates responses using a fine-tuned language model.
- **Environment Variable Management**: Securely handles API keys using a `.env` file.

### Prepare the Dataset
1. Ensure your dataset (`InfoHealthFood_20241225.xlsx`) is placed in the project directory.
 The dataset is sourced from the Taiwan Food and Drug Administration (TFDA) website: [https://consumer.fda.gov.tw/Food/InfoHealthFood.aspx?nodeID=162](https://consumer.fda.gov.tw/Food/InfoHealthFood.aspx?nodeID=162).
2. The dataset should contain the following columns:
   - `許可證字號`: Product ID
   - `中文品名`: Product Name
   - `保健功效`: Health Benefits
## Example Query
```text
Enter a product name to check its health benefits (or type 'exit' to quit):
什麼可以調血脂
Response:
  - e脂100膠囊 的保健功效是: 調節血脂
  - 健康調合油 的保健功效是: 調節血脂
  - 無加糖鮮豆漿 的保健功效是: 調節血脂功能
```
## Acknowledgments
- **OpenAI** for embeddings and GPT-2 model.
- **Qdrant** for vector search capabilities.
- **Hugging Face** for transformer models.


