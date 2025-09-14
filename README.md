# PDF Word Search & Extractor

This is a desktop application designed to streamline the process of searching through multiple PDF files for specific keywords. The application offers a simple graphical user interface (GUI) to help users quickly find relevant documents and extract matching pages into new, organized PDF files. It's particularly useful for researchers, analysts, or anyone who needs to quickly parse through a large number of documents.

The application is built using the following key technologies:

PyMuPDF (fitz): A highly performant library for reading, manipulating, and rendering PDF documents.

customtkinter: A modern and customizable toolkit that extends tkinter, providing a sleek and user-friendly GUI.

Key Features
Intuitive GUI: A clean and straightforward interface allows you to select folders, enter keywords, and configure search options with ease.

Flexible Keyword Search: Search for one or more keywords across an entire folder and its subdirectories. Keywords are not case-sensitive by default.

Regular Expression Support: Enable advanced search queries by treating keywords as regular expressions, allowing for complex pattern matching.

PDF Extraction: Automatically create new PDF files containing only the pages that contain a match, filtering out irrelevant content.

Consolidated Output: Option to combine all matched pages from a search into a single, unified PDF document.

Automatic Highlighting: When creating new PDFs, the application will automatically highlight the search keywords on the extracted pages, making it simple to locate the matches.

Requirements
To run this application, you must have Python installed (version 3.7 or newer is recommended). You will also need to install the two primary libraries used in the project.

You can install the dependencies by running the following command in your terminal or command prompt:

pip install PyMuPDF customtkinter

Getting Started
1. Installation
The easiest way to get the application running is to save the provided Python script as pdf_extractor.py.

It is highly recommended to use a virtual environment to manage your project dependencies and avoid conflicts with other Python projects.

# Create a new virtual environment
python -m venv myenv

# Activate the virtual environment
# On Windows:
myenv\Scripts\activate
# On macOS/Linux:
source myenv/bin/activate

# Install the dependencies inside the virtual environment
pip install PyMuPDF customtkinter

2. Running the Application
Once your dependencies are installed, you can start the application by running the script from your terminal:

python pdf_extractor.py

How to Use
The application's interface guides you through the process step-by-step.

Select Folders:

Click the "Browse..." button to choose the main folder you want to search. The application will recursively search all PDF files within this folder and its subdirectories.

Optionally, select an Output Folder where the new PDF files will be saved. If left blank, the extracted PDFs will be placed in the same directory as the original files.

Enter Search Words:

In the "Words to Search" field, type the keywords you're looking for. Separate each word with a comma (e.g., report, financial, Q4 results).

Choose Options:

Trim spaces: This option automatically cleans up any extra spaces around your keywords.

Use Regex: Check this box to enable regular expressions for more advanced pattern matching.

Create new PDF(s): This is the main extraction feature. The application will generate new PDF files from the pages that contain a match.

Combine all results into one PDF: If the "Create new PDF(s)" option is selected, this will merge all matched pages from all documents into a single, comprehensive output PDF.

Highlight Matches: This will automatically add a yellow highlight to the keywords on the extracted pages.

Start the Search:

Click the "Search PDFs" button to begin the process. The progress bar will update as each file is processed.

The "Results" text box at the bottom will provide a log of which files and pages had matches.

Troubleshooting
Application is not responding: If you're searching a large number of files, the application may appear to freeze briefly. The search operation runs on a separate thread, so please be patient and wait for the progress bar to complete.

File not found errors: Double-check that the folder paths you entered are correct and that the application has the necessary permissions to access them.
