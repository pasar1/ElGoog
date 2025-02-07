# Project Elgoog - Mini Search Engine

![411029766-556ffe33-9a98-4d49-801b-1e297679ae6c](https://github.com/user-attachments/assets/35927133-77a1-435c-9bb5-9f28c822dde8)

## Overview
This project, "Elgoog," is a mini search engine that efficiently performs phrase searches across a collection of documents. It is implemented in Java and runs as a fully functional website using Spring Boot!

## Why I Made This

I developed this project with the goal of helping students and educators easily locate the information they need in their syllabuses and study materials. I know traditional search tools can sometimes be slow when you're trying to find specific phrases in big documents, so I created this tool to deliver quick and precise search results. It’s my hope that this project makes it easier for students to organize and access their coursework effectively!

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

## How It Works
- **Indexing**: Documents are processed into an efficient index structure at startup or via the `/reindex` service.
- **Searching**: Uses the index to quickly find exact phrase matches instead of scanning all documents.
- **Performance**: Designed to outperform naive search implementations in both accuracy and speed.

## Testing
- **Unit Tests**: Validate individual components like the indexer and searcher.
- **Integration Tests**: Ensure indexing and searching work together correctly.
- **End-to-End (E2E) Testing**: Run the web app locally and perform searches through the browser.

## Contributions
Feel free to contribute by improving search efficiency, adding tests, or enhancing the web interface.


### Author
Sam Pasarakonda

