# Wikipedia Search Engine

This search engine aims to index and retrieve Wikipedia articles with a focus on optimizing both result accuracy and retrieval time. The following scoring methods are implemented:

- **TF-IDF**
- **Cosine similarity**
- **BM25**
- **Query expansion**
- **Binary scoring**
- **Page rank**
- **Page views**

## Project Structure

- **se.py**  
  Contains the initialization of the search engine, loading of related indices, and all search methods (BM25, cosine similarity, etc.) and required functions.

- **search_frontend.py**  
  A Flask wrapper for handling and responding to HTTP requests.

- **se_test.py**  
  A testing script that runs queries, returning precision, latency, and other performance metrics.

- **unit_tests.ipynb**  
  A notebook that runs optimization modules and tests different parameters to improve engine performance.

- **inverted_index_gcp.py**  
  Provides readers and writers for interacting with indices and binary files stored in Google Cloud buckets.

## Inverted Indices & Files in Google Cloud Buckets

- Anchor inverted index  
- Title inverted index (with and without stemming, and with bigrams)  
- Body inverted index (with and without stemming, and with bigrams)  
- Body inverted index without popular words filtering  
- Corpus Pickles  

Links to these files are included in the accompanying project report.

---

**Thank you for using the Wikipedia Search Engine!**
