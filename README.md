**PubMed Article Summarizer:**

This project is a web application built using Flask that allows users to upload PubMed articles in text format, preprocesses the text, and summarizes the content using an extractive summarization method. The summarization is performed using the TextRank algorithm from the sumy library.

**Features**

**Upload PubMed Articles:** Users can upload text files containing PubMed articles.

**Text Preprocessing**: The application preprocesses the text by expanding contractions, converting to lowercase, removing punctuation, numbers, and stopwords, and lemmatizing the words.

**Extractive Summarization:** The application summarizes the content of the articles using the TextRank algorithm.

**Display Original and Summarized Text:** The original and summarized articles are displayed on the web page.


**Installation:**

**Prerequisites**
Ensure you have Python 3.6 or later installed. You'll also need to install the following Python packages:


Flask

sumy

nltk

contractions


**Directory Structure:**
The project directory should have the following structure:

project/

│
├── app.py

├── templates/

│   └── index.html

└── uploads/


**Uploading and Summarizing Articles**
**1)** Click the "Choose File" button to select a text file containing a PubMed article.

**2)** Click the "Upload" button to upload the file.

The original article text and the summarized text will be displayed on the page.

**Project Files**

**1)** app.py
The main Flask application file. It contains the logic for handling file uploads, preprocessing the text, summarizing the text, and rendering the HTML templates.


**2)** templates/index.html
The HTML template for the web application's interface. It includes the form for uploading files and displays the original and summarized text.

**Preprocessing Steps:**

**Expand contractions:** Converts contractions like "can't" to "cannot".

**Convert to lowercase:** Standardizes text to lowercase.

**Remove punctuation:** Eliminates punctuation marks.

**Remove numbers:** Removes numerical characters.

**Remove whitespace:** Trims and reduces multiple spaces to a single space.

**Tokenize:** Splits the text into words.

**Remove stopwords:** Removes common English words that do not contribute much meaning (e.g., "and", "the").

**Lemmatize:** Reduces words to their base or root form (e.g., "running" to "run").

**Summarization Method**


The application uses the TextRank algorithm for extractive summarization. This method identifies and extracts the most important sentences from the text to form a concise summary.



**Acknowledgments**

Flask

sumy

nltk
