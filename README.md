# Customer Support Ticket Routing using NLP

## Project Overview

This project is a simple Natural Language Processing (NLP) system that automatically routes customer support tickets to the appropriate department.

The system analyzes the ticket text, matches relevant keywords with predefined support categories, and identifies named entities using spaCy.

## Support Categories

* Billing Team
* Technical Team
* Refund Team
* Sales Team

## Technologies Used

* Python
* spaCy
* Natural Language Processing (NLP)

## How It Works

The project follows these steps:

1. Load the spaCy NLP pipeline.
2. Create sample customer support tickets.
3. Define keywords for each support category.
4. Process each ticket using spaCy.
5. Convert the ticket text to lowercase.
6. Match ticket keywords with category keywords.
7. Calculate a score for each category.
8. Perform Entity Recognition using spaCy.
9. Select the category with the highest score.
10. Route the ticket to the appropriate team.

## Example

### Input

```text
My payment failed.
```

### Output

```text
Scores: {'Billing Team': 1, 'Technical Team': 0, 'Refund Team': 0, 'Sales Team': 0}
Entities: []
Routed To: Billing Team
```

Another example:

```text
Need refund for my order.
```

Output:

```text
Routed To: Refund Team
```

## Project Structure

```text
customer-support-ticket-routing-nlp/
│
├── ticket_routing.py
└── README.md
```

## Installation

Install spaCy:

```bash
pip install spacy
```

Download the English spaCy model:

```bash
python -m spacy download en_core_web_sm
```

## Run the Project

```bash
python ticket_routing.py
```

## Key NLP Concepts

* NLP Pipeline
* Keyword Matching
* Text Processing
* Entity Recognition
* Text Classification
* Automated Ticket Routing

## Future Improvements

This project can be improved by using:

* spaCy Matcher
* Text Similarity
* Machine Learning classification
* TF-IDF
* Word Embeddings
* Transformer-based models
* User input for real-time ticket classification

## Learning Outcome

This project helped me understand how NLP can be used to process customer messages and automatically route them to the appropriate support team.
