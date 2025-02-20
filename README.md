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

The Bookmaking Agent converts syllabus PDFs into structured educational books using AI-generated content.

### Features
- PDF syllabus parsing
- AI-powered content generation
- Professional document formatting
- Automated chapter and topic organization
- Review questions generation

### Running the Bookmaking Agent
1. Place your syllabus PDF in the same directory
2. Update the PDF filename in the script
3. Run:
   ```bash
   python bookmaking_agent.py
   ```

### Output
- Generates a professionally formatted Word document
- Includes table of contents
- Chapter introductions
- Detailed topic content
- Review questions
- Consistent styling

### Note
Both agents require a Google API key with access to the Gemini model. Make sure to handle your API key securely and never commit it to version control.

Remember to always activate the virtual environment before running the agents:
```bash
# Windows
.\venv\Scripts\activate

# Linux/Mac
source venv/bin/activate
```
