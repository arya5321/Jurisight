
# Jurisght

**Jurisght** is a legal document summarization and analysis platform that helps legal professionals streamline document review, assess petition validity, and retrieve relevant case law. It leverages advanced NLP models and machine learning to provide accurate summaries, case success predictions, and an interactive Q&A chatbot.

## Features

- **Legal Document Summarization**: Utilizes Longformer to efficiently summarize extensive legal texts.
- **Case Law Retrieval**: Finds and retrieves relevant case laws based on input queries to support legal research.
- **Petition Validity Testing**: Predicts case success/failure likelihood based on historical data.
- **Chatbot with Retrieval-Augmented Generation (RAG)**: Offers context-aware responses by combining retrieval with generation.
- **Responsive UI**: Built with React for a smooth, interactive user experience.

## Technology Stack

### Frontend Development - React
React powers a responsive, dynamic interface, providing fast-loading pages and reusable components.

### Backend Development & Database - Express.js & MongoDB
- **Express.js**: Manages requests and API endpoints.
- **MongoDB**: Stores legal documents and case law data, utilizing a flexible document-based structure.

### AI/DS Module Development
- **Longformer**: Summarizes large documents, capturing essential insights.
- **RAG (Retrieval-Augmented Generation)**: Enhances chatbot responses by integrating retrieval for higher accuracy.
- **Case Law Retrieval**: Searches for relevant case laws based on query terms, helping users quickly locate supporting cases.
- **Petition Validity Testing**: A machine learning model trained to predict case outcomes based on previous court data.

## Getting Started

### Prerequisites

- Node.js & npm
- MongoDB
- Python 3.8+

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Jurisight/major-project.git
   cd jurisght
   ```

2. Install backend dependencies:
   ```bash
   npm install
   ```

3. Set up and start the MongoDB database.

4. Start the server:
   ```bash
   npm start
   ```

5. (Optional) To start the frontend:
   ```bash
   cd frontend
   npm install
   npm start
   ```

## Usage

1. Upload a legal document for summarization.
2. Use the chatbot for interactive Q&A with accurate, retrieval-augmented responses.
3. Enter queries for **case law retrieval** to find relevant legal precedents.
4. Test petition validity for case success probability.

## Contributing

We welcome contributions! Please fork the repository and submit a pull request with your suggested changes.


