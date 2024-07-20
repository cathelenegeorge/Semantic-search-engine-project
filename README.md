# Semantic-search-engine-project
Semantic search transcends the limitations of traditional keyword searches by understanding the context and nuances of language in user queries. A functional semantic search engine that not only understands the subtleties of human language but also fetches information that truly matters.
### Workflow:
The project can be broke down into the following steps as mentioned below:
 1.text preprocessing to enhance data quality. 
 2.Use the Universal Sentence Encoder to convert text into a format that machines understand. 
 3.Harness the efficiency of FAISS, a library built for rapid similarity search, to compare and retrieve information.
 
### What are the Required Libraries?
tensorflow: The core library for TensorFlow, required for working with the Universal Sentence Encoder.
tensorflow-hub: A library that makes it easy to download and deploy pre-trained TensorFlow models, including the Universal Sentence Encoder.
faiss-cpu: A library for efficient similarity search and clustering of dense vectors.
numpy: A library for numerical computing, which we will use to handle arrays and matrices.
scikit-learn: A machine learning library that provides various tools for data mining and data analysis, useful for additional tasks like data splitting and evaluation metrics.
Understanding Semantic Search
When we're looking to build a semantic search engine, it's important to start with the basics. Let's break down what semantic search is and why it's a game-changer in finding information.

### What is Semantic Search?
Semantic search transcends the limitations of traditional keyword searches by understanding the context and nuances of language in user queries. At its core, semantic search:

Enhances the search experience by interpreting the intent and contextual meaning behind search queries.
Delivers more accurate and relevant search results by analyzing the relationships between words and phrases within the search context.
Adapts to user behavior and preferences, refining search results for better user satisfaction.
How Semantic Search Works - The Simple Version
Now, how does this smart assistant do its job? It uses some clever tricks from a field called Natural Language Processing, or NLP for short. Here’s the simple version of the process:

1.Getting the Gist: First up, the search engine listens to your query and tries to get the gist of it. Instead of just spotting keywords, it digs deeper to find the real meaning.
2.Making Connections: Next, it thinks about all the different ways words can be related (like "doctor" and "physician" meaning the same thing). This helps it get a better sense of what you're asking for.
3.Picking the Best: Finally, it acts like a librarian who knows every book in the library. It sorts through tons of information to pick what matches your query best, considering what you probably mean.

The Technical Side of Semantic Search
After understanding the basics, let's peek under the hood at the technical engine powering semantic search. This part is a bit like math class, where we learn about vectors — no, not the ones you learned in physics, but something similar that we use in search engines.

### Vectors: The Language of Semantic Search
In the world of semantic search, a vector is a list of numbers that a computer uses to represent the meaning of words or sentences. Imagine each word or sentence as a point in space. The closer two points are, the more similar their meanings.

Creating Vectors: We start by turning words or sentences into vectors using models like the Universal Sentence Encoder. It's like giving each piece of text its unique numerical fingerprint.
Calculating Similarity: To find out how similar two pieces of text are, we measure how close their vectors are in space. This is done using mathematical formulas, such as cosine similarity, which tells us how similar or different two text fingerprints are.
Using Vectors for Search: When you search for something, the search engine looks for the vectors closest to the vector of your query. The closest vectors represent the most relevant results to what you're asking.
How Vectors Power Our Search
Vectors are powerful because they can capture the subtle meanings of language that go beyond the surface of words. Here's what happens in a semantic search engine:

Vectorization: When we type in a search query, the engine immediately turns our words into a vector.
Indexing: It then quickly scans through a massive index of other vectors, each representing different pieces of information.
Retrieval: By finding the closest matching vectors, the engine retrieves information that's not just textually similar but semantically related.

### What does the Universal Sentence Encoder do?
The Universal Sentence Encoder (USE) takes sentences, no matter how complex, and turns them into vectors. These vectors are arrays of numbers that capture the essence of sentences. Here's why it's amazing:
Language Comprehension: USE understands the meaning of sentences by considering the context in which each word is used.
Versatility: It's trained on a variety of data sources, enabling it to handle a wide range of topics and sentence structures.
Speed: Once trained, USE can quickly convert sentences to vectors, making it highly efficient.
How does the Universal Sentence Encoder work?
The magic of USE lies in its training. It uses deep learning models to digest vast amounts of text. Here’s what it does:
Analyzes Words: It looks at each word in a sentence and the words around it to get a full picture of their meaning.
Understands Context: It pays attention to the order of words and how they're used together to grasp the sentence's intent.
Creates Vectors: It converts all this understanding into a numeric vector that represents the sentence.

### What is FAISS and what does it do?
FAISS, developed by Facebook AI, is a library for efficient similarity search. After we have vectors from USE, we need a way to search through them quickly to find the most relevant ones to a query. FAISS does just that:
1.Efficient Searching: It uses optimized algorithms to rapidly search through large collections of vectors.
2.Scalability: It can handle databases of vectors that are too large to fit in memory, making it suitable for big data applications.
3.Accuracy: It provides highly accurate search results, thanks to its advanced indexing strategies.

How does FAISS work?
FAISS creates an index of all the vectors, which allows it to search through them efficiently. Here's a simplified version of its process:
1.Index Building: It organizes vectors in a way that similar ones are near each other, making it faster to find matches.
2.Searching: When you search with a new vector, FAISS quickly identifies which part of the index to look at for the closest matches.
3.Retrieving Results: It then retrieves the most similar vectors, which correspond to the most relevant search results.

### Putting it all together:

With USE and FAISS, we have a powerful duo. USE helps us understand language in numerical terms, and FAISS lets us search through these numbers to find meaningful connections. Combining them, we create a semantic search engine that's both smart and swift.
