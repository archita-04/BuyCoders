# BuyCoders – System Design Document

## 1. System Overview

BuyCoders is a cloud-enabled AI-based recommendation system that processes user queries, analyzes product and review data, and returns ranked and explainable product suggestions.

---

## 2. System Architecture

### Presentation Layer
- Web-based user interface
- Accepts user query
- Displays recommendation results

### Application Layer (Flask Backend)
- REST API for handling requests
- Input validation
- Business logic orchestration

### Data Layer
- Product dataset
- Review dataset
- Price history data
- Platform mapping

### AI Engine
- Natural Language Processing using spaCy
- Review filtering
- Sentiment analysis using VADER
- Product ranking algorithm

### Cloud Infrastructure (AWS – Future Ready)
- EC2 for backend hosting
- S3 for dataset storage
- Lambda for scheduled updates

---

## 3. Process Flow

User Query  
→ NLP processing (intent, budget, category)  
→ Fetch product & review data  
→ Review filtering  
→ Sentiment analysis  
→ Product ranking  
→ Explainable recommendation  
→ Display results  

---

## 4. Technology Stack

- Python
- Flask
- Pandas
- spaCy
- VADER Sentiment Analysis
- SQLite / CSV Dataset
- AWS EC2 (deployment)
- AWS S3 (storage)

---

## 5. Data Flow

1. User submits a query
2. NLP engine extracts key parameters
3. Product and review data is retrieved
4. Reviews are filtered and analyzed
5. Products are ranked using scoring logic
6. Output generator creates explainable results
7. Response is returned to the user interface

---

## 6. Scalability Plan

- Multi-category product support
- Real-time price tracking
- Advanced AI ranking model
- Mobile application interface
