# Markdown to Google Docs Converter

This Python script converts markdown meeting notes into a well-formatted Google Document using the Google Docs API.

## Features
- Converts Markdown headers to Google Docs headings (H1, H2, H3).
- Maintains nested bullet point hierarchy.
- Converts `- [ ]` checkboxes into actual checkboxes in Google Docs.
- Highlights mentions (e.g., @name) in **bold**.
- Formats footer notes distinctly.

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/Amulya78364/Markdown-to-GoogleDocs.git
2. Open convert_markdown_to_docs.ipynb in Google Colab.
3. Run the script and authenticate Google Docs API.
4. The generated document link will be printed in the output.

## Dependencies
google-auth
google-auth-oauthlib
google-auth-httplib2
google-api-python-client

## How to Run in Google Colab
1. Open Google Colab: Go to Google Colab.
2. **Upload the Notebook:**
   - Click on **File > Upload Notebook.**
   - Upload the **convert_markdown_to_docs.ipynb** file from the repository.
3. **Install Dependencies:** Run the following command in the first code cell to install the required libraries:
   - !pip install google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client
4. **Authenticate with Google Docs API:**
-The script includes a step to authenticate with your Google account.
-Once you run the script, a link will be generated for authentication. Click the link, sign in to your Google account, and paste the authorization code back into the Colab notebook.
5. **Run the Script:**
-The script will automatically:
--Parse the provided Markdown notes.
--Create a new Google Doc.
--Format the document with the specified styles.

