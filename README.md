# Advanced Sentiment Analysis Dashboard

## Overview
This project is an Advanced Sentiment Analysis Dashboard built using Streamlit and LangChain. It leverages various Large Language Models (LLMs) through Ollama to perform sentiment analysis on user-provided text or batch inputs via CSV files.



## Features
- Single text and batch sentiment analysis
- Multiple LLM model selection (including TinyLlama, Llama2, Phi3, Mistral, and many more)
- Interactive visualizations:
  - Sentiment gauge charts
  - Word clouds
  - Overall sentiment distribution bar charts
- Batch analysis with CSV file upload
- Sample CSV download for batch analysis testing
- Detailed error handling and debugging output

## Installation

### Prerequisites
- Python 3.7+
- Ollama (with desired models installed)

### Installing Ollama
1. Windows
  - Download the Ollama installer from the official Windows page.
  - Run the installer and follow the setup instructions.
  - After installation, restart your terminal and verify installation with:

```
ollama --version
```
- To run the Ollama server:

```
ollama serve
```
2. macOS
- Open Terminal and run:

```
curl -fsSL https://ollama.com/install.sh | sh
```
- After installation completes, verify with:

```
ollama --version
```
- Start the server:

```
ollama serve
```
3. Linux
- Open your terminal and run:

```
curl -fsSL https://ollama.com/install.sh | sh
```
- Verify installation:

```
ollama --version
```
- To start Ollama:
```
ollama serve
```
### Note: After installing, ensure ollama is available in your system PATH. You might need to restart your terminal or system for the command to be recognized.

### Setup
1. Clone the repository:
   ```
   git clone https://github.com/imanoop7/Sentiment-Analysis-Dashboard
   cd sentiment-analysis-dashboard
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. Ensure you have Ollama installed and the desired models downloaded.

## Usage

1. Run the Streamlit app:
   ```
   streamlit run app.py
   ```

2. Open your web browser and navigate to the URL provided by Streamlit (usually `http://localhost:8501`).

3. Use the dashboard:
   - Select an LLM model from the sidebar
   - Enter text in the input area or upload a CSV file for batch analysis
   - Click "Analyse Sentiment" to process the input
   - View the results, including sentiment classification, visualisations, and overall statistics

## Project Structure

- `app.py`: Main Streamlit application file
- `requirements.txt`: List of Python dependencies
- `README.md`: Project documentation (this file)

## Dependencies

- streamlit
- langchain
- langchain-community
- ollama
- plotly
- wordcloud
- matplotlib
- pandas
- nltk

## Notes

- The availability and performance of models may vary depending on your Ollama installation.
- Not all models are optimised for sentiment analysis tasks. Results may vary between different models.



## License

This project is open-source and available under the [MIT License](LICENSE).

