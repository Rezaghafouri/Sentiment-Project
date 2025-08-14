# Iran Khodro Sentiment Analysis Project

## Overview
This project implements an intelligent sentiment analysis system that tracks and analyzes public sentiment about Iran Khodro (ایران خودرو) using real-time news sources. The system combines advanced LLM capabilities with web search functionality to provide detailed sentiment scoring and analysis.

## Features
- Real-time news sentiment analysis
- Detailed source-by-source breakdown
- Numerical sentiment scoring (1-10 scale)
- Automated web searching and content aggregation
- Structured output with reasoning
- Results export to text file

## Technology Stack
- **LLM**: Meta Llama 4 Maverick 17B (via Groq)
- **Search Engine**: Tavily Search API
- **Framework**: LangGraph for workflow management
- **Environment Management**: Python dotenv
- **Output Format**: Both console and text file output

## Project Structure
```
Sentiment Project/
├── Sentiment_Analysis/
│   └── Sentiment_bot.ipynb
├── README.md
├── requirements.txt
└── pyproject.toml
```

## Sentiment Scoring Scale
The project uses a comprehensive 1-10 sentiment scale:
- **1-3**: Very Negative
- **4-5**: Slightly Negative
- **6**: Neutral
- **7-8**: Slightly Positive
- **9-10**: Very Positive

## Setup
1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up environment variables:
   - Create a `.env` file
   - Add your API keys:
     ```
     TAVILY_API_KEY=your_key_here
     ```
4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

## How It Works
1. The system searches for recent news about Iran Khodro using Tavily Search
2. For each news source found:
   - Extracts key information
   - Analyzes sentiment
   - Provides a numerical score
   - Explains the reasoning
3. Results are compiled and saved to 'sentiment_analysis_results.txt'

## Output Format
The analysis provides:
- Source URLs
- Key points from each source
- Individual sentiment scores with explanations
- Overall sentiment score
- Analysis statistics (tokens used, processing time)

## Requirements
- Python 3.8+
- LangGraph
- Groq API access
- Tavily API key
- Required Python packages listed in requirements.txt

## Limitations
- Depends on availability of recent news sources
- Requires active internet connection
- API rate limits may apply
- Results may vary based on available news coverage

## Future Improvements
- Historical trend analysis
- Sentiment visualization
- Multiple language support
- Advanced filtering options
- Automated periodic analysis

## License
[Your chosen license]

## Contributors
[Your name/organization]

## Acknowledgments
- Groq for LLM API
- Tavily for search capabilities
- LangGraph team for the workflow framework
