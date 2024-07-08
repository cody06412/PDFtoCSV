# Text Extraction from PDFs

<img src="Cover Image.png" width="950" height="500">

In this repo, I will provide a comprehensive guide on extracting text data from PDF files in Python.
This approach will cover the text extraction for different components in PDFs such as:
- Plain text
- Tables
- Images in the PDF

To achieve that I will use the **PDFMiner** library to perform an initial analysis of the layout of the PDF and identify the proper tool needed for the specific component.
Then based on the component found I will apply the appropriate function and Python Library. 

The output of this process will be a Python dictionary containing information extracted for each page of the PDF file. Each key in this dictionary will present the page number of the document, and its corresponding value will be a list with the following 5 nested lists containing:

1. The text extracted per text block of the corpus
2. The format of the text in each text block in terms of font family and size
3. The text extracted from the images on the page
4. The text extracted from tables in a structured format
5. The complete text content of the page

You can see a flowchart of the process below:

<img src="Text Extraction Flowchart.png" width="500" height="1000">
