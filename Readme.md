# Tweeter Clone

A comprehensive Twitter-like web application built with Django. This project allows users to interact in a social media environment by posting tweets, sharing photos, and managing their profiles. The application is designed with a responsive Bootstrap interface and supports media uploads, making it suitable for learning Django fundamentals and web development best practices.

## Features

### 1. User Registration & Authentication
- Secure user sign-up and login functionality using Django's built-in authentication system.
- Password hashing and validation for enhanced security.
- Session management to keep users logged in across pages.
- Logout functionality to end user sessions safely.

### 2. Tweet Management
- **Create Tweets:** Users can compose tweets with text and optionally attach photos.
- **Edit Tweets:** Users can modify the content or attached photo of their own tweets.
- **Delete Tweets:** Users can remove their tweets from the platform.
- **View Tweets:** All users can browse tweets posted by others in a chronological feed.

### 3. Photo Uploads
- Support for uploading images with tweets using Django's media handling.
- Uploaded photos are stored in a dedicated media directory and displayed alongside tweets.
- Validation for image file types and size.

### 4. Responsive Bootstrap UI
- Clean and modern interface built with Bootstrap for optimal viewing on desktops, tablets, and mobile devices.
- Consistent layout across all pages, including forms, tweet lists, and profile sections.

### 5. Home Page with Developer Profile
- The landing page features an introduction to the developer and project overview.
- Quick access to developer contact information and social profiles.

### 6. Media and Static File Support
- Static files (CSS, JS, images) are organized for efficient loading and caching.
- Media files (user-uploaded images) are served securely and efficiently.

## Project Structure

```plaintext
Django Project
│
│   db.sqlite3
│   manage.py
│   requirements.txt
│
├───Main
│   │   asgi.py
│   │   settings.py
│   │   urls.py
│   │   views.py
│   │   wsgi.py
│   │   __init__.py
│   └───__pycache__
│
├───media
│   └───photos
│           (user-uploaded images)
│
├───static
│   └───images
│           (static assets)
│
├───templates
│       index.html
│       layout.html
│       layout2.html
│
└───tweet
    │   admin.py
    │   apps.py
    │   forms.py
    │   models.py
    │   tests.py
    │   urls.py
    │   views.py
    │   __init__.py
    ├───migrations
    ├───templates
    │   │   tweet_confirm_delete.html
    │   │   tweet_form.html
    │   │   tweet_list.html
    │   └───registration
    │           logged_out.html
    │           login.html
    │           register.html
    └───__pycache__
```

## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Mehta-g1/Django-Tweeter.git
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Apply Migrations**
   ```bash
   python manage.py migrate
   ```

4. **Create a Superuser (Optional)**
   ```bash
   python manage.py createsuperuser
   ```

5. **Run the Development Server**
   ```bash
   python manage.py runserver
   ```

6. **Access the Application**
   Open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser.

## Developer

**Vikash Kumar Mehta**  
Meerut Institute of Technology (CCSU)  
Email: vikashmehta@mail.com  
GitHub: [github.com/mehta-g1](https://github.com/mehta-g1)  
LinkedIn: [linkedin.com/in/mehta-g1](https://linkedin.com/in/mehta-g1)

## Technologies Used

- **Python:** Core programming language for backend logic.
- **Django:** Web framework for rapid development and clean design.
- **Bootstrap:** Frontend framework for responsive UI.
- **SQLite:** Lightweight database for development and testing.
- **Pillow:** Python Imaging Library for image upload and processing.

## License

This project is provided for educational purposes and learning only.
