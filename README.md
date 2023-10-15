# BizCardX-Data-Extraction

BizCardX is a user-friendly tool for extracting information from business cards using Optical Character Recognition (OCR) technology. This project leverages the EasyOCR library to recognize text on business cards and extracts the data into a SQL database after classification using regular expressions. The extracted information is then accessible through a GUI built using Streamlit. The BizCardX application provides an intuitive interface for users to upload business card images, extract information, and manage the data within a database.

#Overview

BizCardX aims to simplify the process of extracting and managing information from business cards. The tool offers the following features:

    Extraction of key information from business cards: company name, cardholder name, designation, contact details, etc.
    Storage of extracted data in a PostgreSQL database for easy access and retrieval.
    GUI built with Streamlit for a user-friendly interface.
    User options to upload, extract, and modify business card data.

#Libraries/Modules Used

    pandas: Used to create DataFrames for data manipulation and storage.
    psycopg2: Used to store and retrieve data from a PostgreSQL database.
    streamlit: Used to create a graphical user interface for users.
    easyocr: Used for text extraction from business card images.

    Install the required libraries using the command pip install [Name of the library] . Install streamlit, psycopg2, pandas, and easyocr.
    Execute the database_upload.py script using the command streamlit run database_upload.py.
    The web application opens in a browser, presenting the user with the menu options: 'Data Extraction and Modification' and 'About'.
    Users can upload a business card image in the UPLOAD & EXTRACT menu.
    The EasyOCR library extracts text from the uploaded image.
    Extracted text is classified using regular expressions to identify key information such as company name, cardholder name, etc.
    The classified data is displayed on the screen and can be edited by the user if needed.
    Clicking the "Upload to Database" button stores the data in a PostgreSQL database.
    The MODIFY menu allows users to read, update, and delete data in the PostgreSQL database.


