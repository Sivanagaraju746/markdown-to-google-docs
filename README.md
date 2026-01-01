# Markdown to Google Docs Converter

This project converts markdown meeting notes into a formatted Google Doc
using the Google Docs API.

## Features
- Converts markdown headings to Google Docs headings
- Supports nested bullet points
- Converts markdown checkboxes to Google Docs checkboxes
- Styles @mentions
- Applies special formatting for footer content
- Runs in Google Colab with built-in authentication

## How to Run

1. Open Google Colab
2. Upload `markdown_to_google_doc.py`
3. Run the script
4. Authenticate with your Google account when prompted
5. A Google Doc link will be printed in the output

## Requirements
- Google account
- Google Docs API enabled
- Google Colab environment

## Notes
Authentication is handled using `google.colab.auth.authenticate_user()`,
so no credentials file is required.
