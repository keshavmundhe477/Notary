# Notary - Book Reader & Analyzer

**Notary** is a web-based application that allows users to load and read text-based books, analyze word usage, and perform keyword searches. This project is built using HTML, JavaScript, and Bootstrap, offering a clean and responsive interface to display book content and various statistics.

## Features

- **Load Books**: Users can select a book to load and display its contents in the main reading area.
- **Search Functionality**: A search feature allows users to find keywords within the text, highlighting matches and displaying the number of occurrences.
- **Word Usage Analysis**: The app provides an analysis of the book's most and least frequently used words (excluding common stop words).
- **Document Statistics**: Displays basic statistics about the loaded book, including character count, word count, and document length.
- **Smooth Scrolling**: Ensures a smooth reading experience by scrolling to search results.

## Tech Stack

- **HTML5**: Used for structuring the webpage and layout.
- **JavaScript (Vanilla JS)**: Handles dynamic content loading, search functionality, and word analysis.
- **Bootstrap 4**: Provides a responsive design and pre-styled components.
- **FontAwesome**: For additional icons in the interface.

## How It Works

1. **Loading Books**: 
   - The books are stored as `.txt` files, and the user can load them by clicking on the book titles listed in the sidebar.
   - Upon loading, the book content is fetched via an XMLHttpRequest, cleaned (line breaks replaced with HTML `<br>`), and displayed in the main content area.

2. **Search Functionality**:
   - Users can search for any keyword within the loaded book.
   - The search term is highlighted within the text, and the page scrolls to the first match.

3. **Word Usage Analysis**:
   - The app calculates the most and least frequently used words in the book, excluding common stop words.
   - These results are displayed in separate sections, listing the word and the number of occurrences.

4. **Document Statistics**:
   - Character count, word count, and document length are calculated and displayed to give a quick overview of the book.

## Project Structure

├── /books/                  # Contains the book files in .txt format
├── /images/                 # Stores any images used in the project
├── /css/                    # Stylesheets
│   └── style.css            # Main CSS file for custom styles
├── /js/                     # JavaScript files
│   ├── SearchString.js      # Contains search functionality
│   └── main.js              # Core JS to handle book loading and analysis
├── index.html               # Main HTML file
└── README.md                # Project README file

## Usage

1.**Clone the Repository**

git clone https://github.com/your-username/notary-book-reader.git
cd notary-book-reader

2.**Run the Application**

-Open the index.html file in any web browser to use the app locally.

3.**Add More Books**
-Place .txt files of new books in the /books/ folder and update the sidebar with their filenames.

## Future Improvements

-Add support for more file formats (e.g., .epub or .pdf).
-Implement bookmarking and progress tracking features.
-Enhance the word analysis to provide more detailed insights (e.g., word clouds or n-gram analysis).
