# Shayri Generator Web Application

This project is a Flask-based web application that generates Shayri (poetry) using the Google Generative Language API (Gemini-Pro). It provides a simple web interface where users can enter a prompt and receive generated English-written Hindi-style Shayri.

---

## Overview

The application runs a Flask server that:

* Serves a styled web interface for entering a Shayri prompt
* Sends the user prompt to the Gemini-Pro API for text generation
* Displays the generated Shayri on a separate result page
* Includes basic logging and content safety checks

---

## Features

* Web UI to input a Shayri prompt
* Generates Shayri using Gemini-Pro text generation API
* Displays the generated output on a clean results page
* Basic safety filtering based on API safety ratings
* Styled and structured frontend pages

---

## Tech Stack

* **Backend:** Python, Flask
* **HTTP Client:** Requests
* **Frontend:** HTML, CSS
* **API:** Google Generative Language API (Gemini-Pro)

---

## Project Structure

```
Shayri-Generator-main/
│
├── app.py                     # Flask app and API logic
├── requirements.txt           # Project dependencies
│
├── templates/                 # HTML templates
│   ├── index.html             # Input page
│   └── result.html            # Result display page
│
└── static/
    └── styles.css             # Application styling
```

---

## Installation

1. Ensure Python is installed.
2. Extract the project folder.
3. Open a terminal in the project directory.
4. Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Configuration

The application requires a valid Gemini-Pro API key.

Open `app.py` and update:

```python
API_ENDPOINT = "https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key=API_Key"
```

Replace `API_Key` with your actual Google Generative Language API key.

---

## Running the Application

Start the Flask server:

```bash
python app.py
```

The application runs in debug mode.
Open your browser and go to:

```
http://127.0.0.1:5000
```

---

## Usage

1. Open the website.
2. Enter a Shayri prompt in the text field.
3. Submit the form.
4. View the generated Shayri on the result page.

---

## Notes

* Internet connection is required.
* A valid Gemini-Pro API key must be configured.
* Generated content is subject to Google safety filtering logic implemented in the application.

---

## License

No license file is included in this project.
