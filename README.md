# Google Docs Markdown Formatter

This project is a Python script designed to convert markdown meeting notes into a well-formatted Google Doc using the Google Docs API. 
It runs in **Google Colab** and automates formatting for headings, bullet points, checkboxes, and more.
The script ensures your markdown content is neatly organized in a Google Doc with proper styles.

---

## **Brief Description**

The project takes markdown meeting notes and:
- Converts them into a Google Doc.
- Formats the content:
  - Main title as Heading 1.
  - Section headers as Heading 2.
  - Sub-section headers as Heading 3.
  - Nested bullet points with proper indentation.
  - Markdown checkboxes (`- [ ]`) converted into actual Google Doc checkboxes.
  - Mentions like `@name` highlighted with distinct styling.

It uses **Google Docs API** to create and update the Google Doc programmatically.

---

## **Setup Instructions**

1. **Enable the Google Docs API**:
   - Go to the [Google Cloud Console](https://console.cloud.google.com/).
   - Create a new project (or use an existing one).
   - Search for and enable the **Google Docs API** for your project.
   - If running locally:
     - Create a **service account** under **IAM & Admin**.
     - Download the service account JSON file.
     - Store it securely on your machine.

2. **Open the Colab Notebook**:
   - Open the provided Colab notebook: [Google Docs Markdown Formatter](https://colab.research.google.com/drive/1J3AWbgFcO9dnH6zlEogyOw8_LKMD7REe#scrollTo=Uh2oE0fKzhDl).
   - Authenticate your Google account when prompted.

3. **Run the Notebook**:
   - Follow the steps in the notebook to:
     - Paste your markdown content.
     - Authenticate with Google Docs API.
     - Generate a formatted Google Doc.

---

## **Required Dependencies**

No additional installations are needed in **Google Colab**, but if running locally, install these libraries:
- `google-auth`
- `google-auth-oauthlib`
- `google-api-python-client`

Install them via:
```bash
pip install google-auth google-auth-oauthlib google-api-python-client
