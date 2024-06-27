# Buliding-a-RAG-LLM
## What is RAG?

RAG stands for Retrieval Augmented Generation. 

- Retrieval : Seeking relevant information from a source given a query. ex: Getting relevant passages of Wikipedia text from a database given a question.

- Augmented : Using the relevant retrieved information to modify an input to a generative model

- Generation : Generating an output given an input. Ex: Generating a passage of text given an input prompt.

## Advantage of using RAG

 - Work with custom data
 - Help LLMs generate more factual outputs

## Key terms:

 - VectorStoreIndex: A class used to create an index that facilitates efficient retrieval of documents based on their vector represantation.
   - Purpose: The primary purpose of VectorStoreIndex is to enable fast and accurate search and retrieval of documents byy converting them  into vector embeddings. This is particularly useful in NLP tasks where simialrity between text documents needs to be measured.
   - Functions:
     Indexing Documents: Converts text documents into vector embeddings and stores them in a searchable index.
     Vector-Based Retrieval: Enables querying the index to find documents that are similar to a given query vector.
     Efficiency: Optimizes search operations to quickly retrieve relevant documents from potentially large datasets.
   - How it works:
     1. Document Embedding: Each document is converted into a vector using an embedding model (sentence transformers)
     2. Index Creation: The resulting vectors are stored in an index structure that supports efficient similarity search (k-nearest neighbors search)
     3. Query Processing: When a query is received, it is also converted into a vector. The index is then searched to find docu,ents with vectors that are most similar to the query vector.
        
 - ServiceContext: A class that encapsulates the configuration and state necessary for service-related tasks, including language model (LLM) interactions and embedding operations.
   - Purpose: It serves as a centralized configuration hub that maintains the state and settings required for various services, such as LLMs and embeddings. It ensures that these services operate consistently and efficiently within a specified context.
   - Functions:
     Configuration Management: Stores settings and parameters needed for initializing and running LLMs and embedding models.
     State Maintenance: Keeps track of the current state of services, such as model instances and embedding configurations.
     Contextual Consistency: Ensures that all components (e.g., LLM, embeddings) operate within a unified context, avoiding mismatches in configurations.
## Prerequistes

 llama-index
 
 openai
 
 pypdf
 
 python-dotenv
 
