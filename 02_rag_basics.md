# Retrieval-Augmented Generation (RAG)

## What is RAG?
Retrieval-Augmented Generation combines information retrieval with a language model. The application first searches a knowledge source for relevant passages, then supplies those passages to the model as context for answering a question.

## Typical workflow
1. Ingest source documents.
2. Extract text from each document.
3. Split long text into overlapping chunks.
4. Index the chunks for semantic search.
5. Retrieve the most relevant chunks for a user question.
6. Generate an answer grounded in the retrieved context.
7. Display source information so the answer can be checked.

## Why chunking matters
Very large passages may contain unrelated information. Very small passages may lose context. Chunk size and overlap should be tested against a representative set of questions.

## Example question
Question: Why does a RAG application retrieve documents before generating an answer?
Answer: Retrieval supplies relevant source material to the model, helping the response stay grounded in the available knowledge.
