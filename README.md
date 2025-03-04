# ScraperBot: Your AI Chat Companion

ScraperBot is an AI-powered chatbot that leverages a Deep Seek model integrated with the Groq API to answer questions based solely on content scraped from a website or extracted from a PDF. Built with Streamlit and various scraping libraries, this application provides an interactive chat interface to explore content in a contextual manner.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Deployment](#deployment)
- [Usage](#usage)

## Overview

ScraperBot allows you to:
- **Scrape Websites:** Extract text content from websites using BeautifulSoup.
- **Process PDFs:** Extract and clean text from PDF files using pdfplumber.
- **Chat with AI:** Interact with a chatbot powered by the Deep Seek model via the Groq API, providing answers based on the scraped content.

The primary application file is `main.py` and all required libraries are listed in `requirements.txt`.

## Features

- **Web and PDF Scraping:** Automatically retrieve and process content from provided URLs or uploaded PDF files.
- **AI-Powered Responses:** Utilize the Groq API and a Deep Seek model to generate context-aware answers.
- **Interactive Chat Interface:** Built with Streamlit, the UI enables an easy-to-use chat experience.
- **Secure API Key Management:** Uses environment variables to securely load the Groq API key.

## Installation

1. **Create an Account and Get an API Key:**
   - Visit [Groq - Fast AI Inference](https://groq.com) and sign up for a free account.
   - After registration, obtain your free API key.

2. **Create a `.env` File:**
   - In the root directory of the project, create a file named `.env`.
   - Copy your API key into this file using the following format:

     ```env
     key=YOUR_API_KEY_HERE
     ```

3. **Set Up Your Virtual Environment:**
   - Create a virtual environment for the project. For example:

     ```bash
     python -m venv venv
     ```

   - Activate the virtual environment:
     - On macOS/Linux:

       ```bash
       source venv/bin/activate
       ```

     - On Windows:

       ```bash
       venv\Scripts\activate
       ```

4. **Install Dependencies:**
   - Install the required Python packages using:

     ```bash
     pip install -r requirements.txt
     ```
## Deployment

 **Run the  Application:**
   - Launch the Streamlit app by running:

     ```bash
     streamlit run main.py
     ```
## Usage

### Scraping a Website
- **Enter a valid website URL** in the provided input field.
- Click **"Scrape Website"** to extract text from the page.

### Processing a PDF
- **Upload a PDF file** using the file uploader.
- Click **"Process PDF"** to extract and clean the text.

### Chat Interface
- Once the content is processed, use the **chat interface** to ask questions.
- The AI responds with information solely based on the scraped or processed content.

### Clear Everything
- Use the **"Clear Everything"** button to reset the application and start fresh.
