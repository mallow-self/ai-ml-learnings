# Vector DB

## Why

- Over 80% of data is unstructured on the internet like images, videos and audio.
- If we need to store it in relational database, we have to give some context like tags, name, category and so on.

## What

- A vector database indexes and stores vector embeddings for fast retrieval and similarity search.

- unstructured_data -> Model(ml) -> vector embedding

- A vector embedding is a list of numbers which represents the data in different way.

- We can represent a word, sentence and a image to get numerical number.

- we can use this number to find euclidean distance(distance between two objects) to find similarity search.

  - d=((x2-x1)^2 +(y2-y1)^2)^1/2

- So if we need to find difference between thousands of embeddings is slow if done on the fly.

- So we need to vector indexing.

## Vector Indexing

- Index is same as index in relational db. It is a data structure which sorts the field of increasing performance of searching capabilities.

## Use cases

1. Long-term memory for LLMs.
2. Semantic search: Search based on the meaning or context.
3. Similarity search for text, images, audio or video data.
4. Recommendation engine - suggestion similar to past purchases.

## Some vector Databases

- Pinecone
- Weaviate
- Chroma
- Redis
- Qdrant
- Milvus
- Vespa

## Fireship video

- A vector is a array of numbers. Embeddings are grouped together based on semantic data.
- Vector db is used to store vector embeddings