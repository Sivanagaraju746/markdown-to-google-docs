# Markdown to Google Docs Converter

## Brief Description
This project contains a Python script that runs in Google Colab and converts
provided markdown meeting notes into a well-formatted Google Doc using the
Google Docs API.

The script programmatically creates a new Google Doc, parses markdown content,
applies appropriate heading styles, maintains nested bullet point hierarchy,
converts markdown checkboxes into Google Docs checkboxes, preserves assignee
mentions with distinct styling, and formats footer information separately.

---

## Setup Instructions
1. Ensure you have a Google account
2. Enable the Google Docs API in Google Cloud Console
3. Open Google Colab
4. Upload the provided Python script or open the included Colab notebook

---

## Required Dependencies
The following dependencies are required and are installed at runtime in
Google Colab:

- google-api-python-client  
- google-auth  
- google-auth-httplib2  
- google-auth-oauthlib  

No local installation or credentials file is required.

---

## How to Run in Google Colab
1. Open Google Colab
2. Upload `markdown_to_google_doc.py` or open `markdown_to_google_doc.ipynb`
3. Run all cells in order
4. Authenticate with your Google account when prompted
5. The script will create a new Google Doc and print the document link in the output

---

## Features Implemented

### Google Docs Integration
- Uses the Google Docs API
- Implements authentication in a Google Colab environment
- Creates a new Google Doc programmatically

### Formatting Requirements
- Main title is formatted as **Heading 1**
- Section headers (e.g., Attendees, Agenda) are formatted as **Heading 2**
- Sub-section headers under Agenda are formatted as **Heading 3**
- Maintains nested bullet point hierarchy with proper indentation
- Converts markdown checkboxes (`- [ ]`, `- [x]`) into Google Docs checkboxes
- Preserves assignee mentions (`@name`) with distinct styling
- Applies distinct styling to footer information (meeting recorded by, duration)

### Code Structure
- Modular and readable code
- Meaningful variable and function names
- Proper error handling using try/except blocks
- Basic documentation and inline comments included

---

## Working Colab Notebook
A working Google Colab notebook (`markdown_to_google_doc.ipynb`) is included in
this repository and demonstrates the complete end-to-end workflow:
- Authentication in Colab
- Markdown parsing
- Google Docs creation and formatting
