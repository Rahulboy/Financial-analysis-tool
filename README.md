Financial Analysis and Reporting Tool
Project Summary
This project is a sophisticated, multi-agent system designed to provide comprehensive financial reports and news sentiment analysis for any publicly traded company. The application leverages a Flask backend to orchestrate a series of specialized agents—a financial researcher, a news researcher, and a sentiment analyst—to deliver a synthesized, human-readable report via a clean, web-based interface.

Key Features
Financial Data Retrieval: Fetches and structures key financial metrics, including current price, market capitalization, and P/E ratio, using yfinance.

Real-time News Search: Utilizes Google Search to find the latest news headlines and relevant articles for a specified company.

Automated Sentiment Analysis: An internal agent analyzes the news headlines to determine the overall sentiment (positive, negative, or neutral).

Synthesized Reporting: Combines all collected financial data, news headlines, and sentiment analysis into a single, cohesive, and easy-to-understand report.

Web-based Interface: The user-friendly frontend allows for a seamless experience—simply enter a stock ticker to generate a new report.

Technology Stack
Backend: Python 3.12, Flask

Agentic Framework: langchain, langgraph

Data Retrieval: yfinance for financial data, requests and BeautifulSoup for web scraping, and langchain_google_community for Google Search API integration.

Frontend: HTML, CSS, JavaScript

Getting Started
To run this project, you will need to set up a Python environment and obtain a Google API key and a Google Custom Search Engine (CSE) ID.

Clone the Repository:

git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
cd financial-analysis-tool

Install Dependencies: Ensure you have Python 3.12 installed. Then, install the required packages using the requirements.txt file.

pip install -r requirements.txt

Configure API Keys:

Set your Google API key and CSE ID as environment variables in your terminal.

Note: If you are on a corporate network or have security restrictions, this may be difficult. The API keys are already hardcoded into main.py for ease of use in a local environment. For public use, it is best practice to move these to environment variables.

Run the Server:

python main.py

The server will start and be available at http://127.0.0.1:8080.

Open the Web Page:
Open the index.html file in your web browser and enter a stock ticker symbol to generate your first report.

File Structure
main.py: The Python Flask backend that runs the multi-agent system and serves the API.

index.html: The HTML frontend that provides the user interface.

requirements.txt: Lists all the necessary Python libraries for the project.

Dockerfile: Provides a blueprint for building a containerized version of the application.

A Special Note
This project was built and debugged in a corporate environment with network and administrative restrictions. The journey to get the project running locally, while challenging, was a valuable exercise in problem-solving and environment management. The successful execution of this project, despite the obstacles, is a testament to the robustness of the application's design and a demonstration of my ability to overcome technical hurdles.
