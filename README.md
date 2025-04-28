# ElGoog - AI-powered Search Engine

![411029766-556ffe33-9a98-4d49-801b-1e297679ae6c](https://github.com/user-attachments/assets/35927133-77a1-435c-9bb5-9f28c822dde8)

## Overview
Elgoog is an optimized phrase search engine designed for high-performance text retrieval across a structured document corpus. Implemented in Java and leveraging Spring Boot, the system is built to execute efficient indexed queries, ensuring sublinear search time complexity through advanced data structures.

## Why I Made This

I built this project to make searching for information in syllabi and academic materials faster and easier. Traditional search methods can be slow and frustrating, especially when you're trying to find an exact phrase. By creating a smarter indexing system, this search engine quickly finds the right information without making you dig through endless text. By implementing an optimized indexing mechanism, the system enables rapid phrase-matching with precise tokenization and lexicographical ordering. My goal is to help students and educators get what they need instantly, making studying and research more efficient and enjoyable! 

## Features
- **Exact Phrase Search**: Returns a sorted list of document IDs that contain the exact search phrase (matching both words and order).
- **Optimized Indexing**: Uses a pre-built index to speed up searches significantly compared to a naive search.
- **Web Interface**: Accessible through a browser, providing an easy-to-use interface for searching documents.
- **API Services**:
  - `http://localhost:8081/` - Main search page
  - `http://localhost:8081/docs` - View all indexed documents
  - `http://localhost:8081/reindex` - Replace the document set

## How to Run
1. **Clone the repository**:
   ```bash
   git clone <repository_url>
   cd mini-search-engine
   ```
2. **Build and run the project**:
   ```bash
   ./mvnw spring-boot:run
   ```
3. **Access the website**:
   - Open `http://localhost:8081` in your browser.
  
## Technologies Used

**Frontend**: 
- Built with HTML, CSS, and JavaScript for a simple yet responsive user interface.

**Backend**:
- Java & Spring Boot: Powers the backend logic for indexing and search operations.
- H2 In-Memory Database: Stores documents and search indices for fast retrieval.

## How It Works
- **Indexing**: Documents are processed into an efficient index structure at startup or via the `/reindex` service.
- **Searching**: Uses the index to quickly find exact phrase matches instead of scanning all documents.
- **Performance**: Designed to outperform naive search implementations in both accuracy and speed.

## Technical Design

- **Indexing Strategy**: The system leverages a positional inverted index, mapping term occurrences to their respective document locations, enabling O(1) lookup for common queries.
- **Search Algorithm**: Utilizes a multi-pass filtering approach with optimized phrase detection, reducing unnecessary I/O operations.
- **Scalability**: Designed to handle dynamic document sets with efficient re-indexing mechanisms.
- **Performance Benchmarks**: Optimized search operations significantly outperform naive sequential scans, achieving a reduction in query execution time by an order of magnitude.

## Testing
- **Unit Tests**: Validate individual components like the indexer and searcher.
- **Integration Tests**: Ensure indexing and searching work together correctly.
- **End-to-End (E2E) Testing**: Run the web app locally and perform searches through the browser.

## Contributions
Feel free to contribute by improving search efficiency, adding tests, or enhancing the web interface!


### Author
Sam Pasarakonda

