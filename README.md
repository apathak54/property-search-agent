# Property Search System with MongoDB and LangChain

This project implements a property search system that allows users to search for properties based on either one-time investment or monthly payment criteria. It uses MongoDB for data storage and LangChain for natural language query processing.

## Features

- Search properties based on one-time investment budget
- Search properties based on monthly payment budget
- Natural language query processing using LangChain
- MongoDB integration for efficient property data storage and retrieval
- Support for multiple EMI options (3, 5, and 7 years)

## Prerequisites

- Python 3.8+
- MongoDB Atlas account
- OpenAI API key

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd property-search-agent
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
Create a `.env` file in the project root with the following variables:
```
OPENAI_API_KEY=your_openai_api_key
```

## Project Structure

- `main.py`: Main application file containing the core logic
- `config.py`: Configuration file with MongoDB connection details and schema information
- `README.md`: This documentation file

## Configuration

The `config.py` file contains:
- MongoDB connection URI
- Database and collection names
- Property schema definition
- Example queries for one-time and monthly payment searches

## Usage

1. Run the application:
```bash
python main.py
```

2. The system currently supports two types of queries:
   - One-time investment: "I am looking for one time investment property with budget X"
   - Monthly payment: "I am looking for monthly payment property with budget Y"

## Example Queries

1. One-time investment search:
```
"I am looking for one time investment property with budget 1000000000"
```

2. Monthly payment search:
```
"I am looking for monthly payment property with budget 120000"
```

## Schema

The property schema includes:
- _id: Unique identifier
- name: Property name
- location: Property location
- totalSqftAvailable: Total square footage
- pricePerSqft: Price per square foot
- totalPrice: Total property price
- threeYear: Monthly EMI for 3 years
- fiveYear: Monthly EMI for 5 years
- sevenYear: Monthly EMI for 7 years

## Author

Anurag

## License

This project is licensed under the MIT License - see the LICENSE file for details. 