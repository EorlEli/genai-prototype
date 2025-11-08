# GenAI Prototype: Customer Reviews Analysis

A Streamlit web application for analyzing customer reviews with sentiment analysis capabilities. This prototype demonstrates how to process and visualize customer feedback data using Python and modern data science libraries.

## Features

- **Data Ingestion**: Load and parse customer review data from CSV files
- **Text Cleaning**: Preprocess review text for analysis
- **Sentiment Analysis**: Analyze sentiment scores of customer reviews
- **Interactive Dashboard**: Filter and explore data by product categories
- **Visualizations**: View sentiment trends and distributions

## Prerequisites

- Python 3.8+
- pip (Python package manager)

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd genai-prototype
   ```

2. Create and activate a virtual environment (recommended):
   ```bash
   python -m venv .venv
   .venv\Scripts\activate  # On Windows
   # or
   source .venv/bin/activate  # On macOS/Linux
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Project Structure

```
genai-prototype/
├── data/
│   └── customer_reviews.csv   # Sample customer review data
├── .env                      # Environment variables
├── app.py                    # Main Streamlit application
├── requirements.txt          # Python dependencies
└── README.md                 # This file
```

## Usage

1. Start the Streamlit application:
   ```bash
   streamlit run app.py
   ```

2. Open your web browser and navigate to the URL shown in the terminal (typically http://localhost:8501)

3. Use the interface to:
   - Ingest the dataset
   - Parse and clean review text
   - Filter reviews by product
   - View sentiment analysis visualizations

## Data Format

The application expects a CSV file with the following columns:
- `PRODUCT`: Name of the product being reviewed
- `DATE`: Date of the review
- `SUMMARY`: The review text
- `SENTIMENT_SCORE`: Numeric sentiment score (-1 to 1)
- `Order ID`: Unique identifier for each review

## Customization

### Environment Variables
Create a `.env` file in the project root to set environment variables:
```
# Example .env file
DEBUG=True
```

### Adding New Features
1. Extend the `clean_text()` function in `app.py` for custom text processing
2. Add new visualizations using the available data
3. Implement additional filtering options

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- Data processing with [pandas](https://pandas.pydata.org/)
- Visualizations powered by [Matplotlib](https://matplotlib.org/) and Streamlit's native charting

---

*This is a prototype application for demonstration purposes.*
