<<<<<<< HEAD
# Project 2
=======
# BookReview
## Introduction:

This book review website facilitates users in searching for books, posting, and viewing reviews and ratings. The website integrates a proprietary database and the Google Books API, offering a collection of over 10,000 books and 20,000 reviews. Users can query the website’s own API, receiving a JSON object containing book details and reviews from both the database and Google Books API, enhancing understanding of concepts like Web Services and REST APIs. The site is deployed on a Flask server, leveraging PostgreSQL for data management.

## Features:

User Registration and Login: Users must register and log in to submit book reviews and ratings. This helps keep track of who submitted each review/rating.
Book Search: Users can search for books using the search feature. The backend gathers data from Google Books API and the website’s PostgreSQL database.
Book Details: When a book is searched, a list of related books is shown with details like author, ISBN number, and publication date.
Reviews and Ratings: Clicking on a specific book shows its detailed information along with user reviews and ratings. Users can add their own ratings and reviews.
API Access: The website provides an API endpoint for others to request reviews and ratings, compensating for the lack of review and rating support in the Google Books API.

## Technologies Used
**Backend**: Flask(Python)<br>
**Database**: PostgreSQL<br>
**API Integration**: Google Books API<br>
**Frontend**: HTML, CSS<br>

## Usage:

User Registration and Login:
Navigate to the registration page to create a new account.
Log in using your credentials.
Search for Books:
Use the search bar to find books. The backend fetches data from Google Books API and the local PostgreSQL database.
View and Submit Reviews and Ratings:
Click on a book to view its details, including reviews and ratings.
Submit your own review and rating using the provided form.
>>>>>>> 31a42ff0293335e3599185ecab2495e6f5baa1ac
