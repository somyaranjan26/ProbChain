# ProbChain [Hashnode blog](https://somyaranjan.hashnode.dev/hack-o-ween)


### Flow
#### app.py
- Initialize the LLMChain with the specified local LLM model file and configuration.
- Initialize the PromptTemplate and HuggingFaceBgeEmbeddings with the specified template and model details.
- Initialize the Chroma vector store and RetrievalQA with the specified vector store and retriever.
- Perform semantic search using the retriever and the user's query.
- Initialize the Gradio interface with the specified input and output settings.
- Launch the Gradio interface.
Outputs
- The semantic search results.
- The response from the question-answering bot in the Gradio interface.

#### Outputs
- The semantic search results.

### Flow
#### ingest.py
- The code imports necessary modules and classes.
- It defines the model name, model kwargs, and encode kwargs for creating the HuggingFaceBgeEmbeddings instance.
- The code creates the embeddings using the specified model and kwargs.
- It initializes the PyPDFLoader with the PDF file name and loads the documents.
- The RecursiveCharacterTextSplitter is instantiated with the chunk size and overlap.
- The code splits the documents into smaller chunks of text using the text splitter.
- The Chroma algorithm is used to create a vector store from the text chunks and embeddings.
- The vector store is created with the specified collection metadata and persist directory.
- The code prints a message indicating that the vector store has been created.
