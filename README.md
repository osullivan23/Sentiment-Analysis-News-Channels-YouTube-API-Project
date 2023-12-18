# YouTube API Project

## Overview

This project explores the relationship between sentiment and popularity in the YouTube content of a news channel, utilising the YouTube API. The analysis involves collecting up-to-date data from selected YouTube channels, cleaning the data for sentiment analysis, and utilising Natural Language Toolkit (nltk) in Python for text processing. The ultimate goal is to understand how the intended sentiment of the content aligns with the audience's reception.

## Project Goals

1. **Data Collection**
   - Create an API client.
   - Develop a framework to extract relevant data from channels of interest using the YouTube API's documentation.
   - Build Pandas DataFrames containing information about videos and comments for each channel.

2. **Data Cleaning**
   - Identify and handle missing data appropriately (remove, interpolate, or extrapolate).
   - Format dates (e.g., convert YYYY-MM-DDTHH:MM:SSZ to the day published).
   - Clean descriptions and comments for sentiment analysis (remove punctuation, emojis, and web addresses).

3. **Distributions of Statistics**
   - Present key statistics about the channels.

4. **Sentiment Analysis**
   - 4.1 **Natural Language Processing (NLP)**
      - Lemmatise text (convert plural forms to singular).
      - Remove stopwords for more meaningful analysis.
      - Part of Speech Tagging (POS) to label each word based on function within text.
      - Named Entity Recognition to identify names, locations, etc.
      - Chunking to group tokens with commonality.
   - 4.2 **VADER Sentimental Analysis**
      - Calculate collective sentiment values.

## Getting Started

### Data Collection - The YouTube API

1. **Register for API Access:**
   - Create a project on the Google Developers Console.
   - Enable the YouTube Data API to obtain API credentials, including an API key.

2. **Understand the API Documentation:**
   - Visit the YouTube Data API documentation for details on endpoints, parameters, response format, and usage guidelines.

3. **Choose the Appropriate Endpoint:**
   - Use the API documentation and a channel's unique ID to locate the data.

4. **Authentication:**
   - Include your API key in API requests for authentication, usually as a parameter in the request URL.

5. **Make HTTP Requests:**
   - Use Python code to make HTTP requests to the API's endpoint. Specify the HTTP method (usually GET) and provide required parameters.

6. **Handle Responses:**
   - Parse JSON responses to extract necessary data. Handle errors and exceptions according to the API documentation.

7. **Rate Limiting:**
   - Stay within YouTube API's rate limits to avoid temporary blocks. Be aware of quotas for different API endpoints and methods.

## Dependencies
- Python
- Natural Language Toolkit (nltk)
- Pandas

## License
This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code as needed. Contributions are welcome!

## Acknowledgements
- Steven Bird, Edward Loper, Ewan Klein for the Natural Language Toolkit (nltk).
- O’Reilly Media Inc. for the book "Natural Language Processing with Python" by Steven Bird, Edward Loper, Ewan Klein.
