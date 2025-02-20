# AI Agents Documentation

This repository contains two AI agents built using LangChain and Google's Gemini model:

## Setup

1. Create and activate a virtual environment:
   ```bash
   # Windows
   python -m venv venv
   .\venv\Scripts\activate

   # Linux/Mac
   python -m venv venv
   source venv/bin/activate
   ```

2. Create a `.env` file and add your Google API key:
   ```
   GOOGLE_API_KEY=your_api_key_here
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Browser Agent

The Browser Agent is designed to automate web browsing tasks using LangChain and Gemini.

### Running the Browser Agent
```bash
python browser_agent.py
```

The agent will:
- Navigate to Reddit
- Search for "browser-use"
- Click on the first post
- Return the first comment

## Bookmaking Agent

The Bookmaking Agent converts syllabus PDFs into structured educational books using AI-generated content. Two versions are available:

### Gemini Version
Uses Google's Gemini model through the official API. Requires a Google API key.

### OpenRouter Version
Uses Qwen-VL-Plus model through OpenRouter API. Requires an OpenRouter API key.

### Features
- PDF syllabus parsing
- AI-powered content generation
- Professional document formatting
- Automated chapter and topic organization
- Review questions generation

### Running the Bookmaking Agent
1. Place your syllabus PDF in the same directory
2. Update the PDF filename in the script
3. Choose which version to run:
   ```bash
   # For Gemini version
   python bookmaking_agent.py

   # For OpenRouter version
   python bookmaking_open_router_agent.py
   ```

### Environment Setup
Create a `.env` file with the appropriate API key:
```bash
# For Gemini version
GOOGLE_API_KEY=your_api_key_here

# For OpenRouter version
OPENROUTER_API_KEY=your_api_key_here
```

### Output
- Generates a professionally formatted Word document
- Includes table of contents
- Chapter introductions
- Detailed topic content
- Review questions
- Consistent styling

### Note
The Gemini version requires a Google API key, while the OpenRouter version requires an OpenRouter API key. Make sure to:
- Handle your API keys securely
- Never commit them to version control
- Choose the version that best fits your needs and API access

Remember to always activate the virtual environment before running the agents:
```bash
# Windows
.\venv\Scripts\activate

# Linux/Mac
source venv/bin/activate
```
