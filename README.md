# BookReview
Introduction:

This book review website facilitates users in searching for books, posting, and viewing reviews and ratings. The website integrates a proprietary database and the Google Books API, offering a collection of over 10,000 books and 20,000 reviews. Users can query the website’s own API, receiving a JSON object containing book details and reviews from both the database and Google Books API, enhancing understanding of concepts like Web Services and REST APIs. The site is deployed on a Flask server, leveraging PostgreSQL for data management.

Features:

User Registration and Login: Users must register and log in to submit book reviews and ratings. This helps keep track of who submitted each review/rating.
Book Search: Users can search for books using the search feature. The backend gathers data from Google Books API and the website’s PostgreSQL database.
Book Details: When a book is searched, a list of related books is shown with details like author, ISBN number, and publication date.
Reviews and Ratings: Clicking on a specific book shows its detailed information along with user reviews and ratings. Users can add their own ratings and reviews.
API Access: The website provides an API endpoint for others to request reviews and ratings, compensating for the lack of review and rating support in the Google Books API.
Technologies Used
Backend: Flask
Database: PostgreSQL
API Integration: Google Books API
Frontend: HTML, CSS, JavaScript

Installation:

Clone the repository:

git clone https://github.com/yourusername/book-review-website.git

Navigate to the project directory:
cd book-review-website

Install the required packages:
pip install -r requirements.txt

Set up the PostgreSQL database:
Ensure PostgreSQL is installed and running.

Create a database and user.
Update the database configuration in config.py.

Run the Flask application:
flask run

Usage:

User Registration and Login:
Navigate to the registration page to create a new account.
Log in using your credentials.
Search for Books:
Use the search bar to find books. The backend fetches data from Google Books API and the local PostgreSQL database.
View and Submit Reviews and Ratings:
Click on a book to view its details, including reviews and ratings.
Submit your own review and rating using the provided form.

API Documentation:

Endpoints
GET /api/books

Description: Retrieve a list of books.
Parameters: search_term (optional) - The term to search for books.
Response: JSON object containing book details.

GET /api/books/<book_id>

Description: Retrieve details of a specific book.
Parameters: book_id - The ID of the book.
Response: JSON object containing book details, reviews, and ratings.

POST /api/reviews

Description: Submit a review and rating for a book.
Parameters: JSON object containing book_id, review, and rating.
Response: JSON object with the status of the submission.
