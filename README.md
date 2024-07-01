# Part 3: Pinecone VectorDB and RAG Pipeline

## Introduction

This part aims to enhance the performance of a standard Question Answering (QA) model by implementing a Retrieval-Augmented Generation (RAG) pipeline. By leveraging relevant documents stored in Pinecone VectorDB, the RAG pipeline provides more accurate and contextually rich answers, reducing hallucinations often produced by standalone QA models.

## Getting Started

To get started, follow the instructions below to set up your environment and run the provided Jupyter notebook.

### Prerequisites

Before running the notebook, ensure you have the following:

- A Pinecone account and API key.
- A Cohere account and API key.
- Python 3.6 or later installed on your system.
- Necessary Python packages: `transformers`, `sentence-transformers`, `datasets`, `cohere`, and `pinecone-client`.

### Installation and Setup

1. **Download the Notebook**: Download the `Part3.ipynb` notebook file for Part 3 of the assignment.

2. **Install Required Packages**: Open a terminal or command prompt, navigate to the directory containing the downloaded notebook, and install the required Python packages:
   ```bash
   !pip install transformers sentence-transformers datasets cohere pinecone-client
   ```

3. **Insert Your API Keys**: Open the Part3.ipynb notebook in Jupyter Notebook or Jupyter Lab. In the specified cells, replace the placeholders with your Pinecone and Cohere API keys:
   - `PINECONE_API_KEY`: Your Pinecone API key.
   - `COHERE_API_KEY`: Your Cohere API key.

4. **Run the Notebook**: Execute each cell in the notebook sequentially. The notebook performs the following tasks:
   - Loads and embeds the `xsum` dataset using `SentenceTransformer`.
   - Creates an index in Pinecone and upserts the document embeddings.
   - Defines functions for retrieving documents and generating answers using the QA model and retrieved context.
   - Evaluates the performance of the RAG pipeline compared to a standard QA model.

5. **View Results**: The output, including generated answers and performance metrics, will be displayed in the notebook cells. Review the results to understand the improvements made by the RAG pipeline.

## Running the Notebook

After setting up your credentials in the notebook:

1. **Execute the Notebook**: Run each cell in the notebook sequentially. The notebook will perform the following tasks:
   - Load and embed the `xsum` dataset using `SentenceTransformer`.
   - Create an index in Pinecone and upsert the document embeddings.
   - Define functions for retrieving documents and generating answers using the QA model and retrieved context.
   - Evaluate the performance of the RAG pipeline compared to a standard QA model.

2. **View Results**: The output will be displayed in the notebook cells. Review the results to understand the improvements made by the RAG pipeline in providing accurate and contextually relevant answers.
