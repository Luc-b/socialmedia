# SimpleSocial (Django Social Network)

SimpleSocial is a social networking web application built with Django. It allows users to sign up, join groups, create posts, and interact with others.

## Features
- **User Authentication**: Register, login, and logout
- **Group Management**: Create, join, and view groups
- **Post Management**: Create, update, and delete posts
- **User-Specific Posts**: View posts by a specific user
- **Additional Pages**: Home page, test page, and thanks page
- **Responsive UI**: Uses Django templates and static files

## Technologies Used
- Python 3
- Django
- SQLite3 (can be replaced with another database)
- Bootstrap (for styling)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/simplesocial.git
   cd simplesocial
   ```
2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```
3. Run database migrations:
   ```bash
   python manage.py migrate
   ```
4. (Optional) Create a superuser account:
   ```bash
   python manage.py createsuperuser
   ```
5. Start the development server:
   ```bash
   python manage.py runserver
   ```
6. Open the application in your browser:
   ```
   http://127.0.0.1:8000/
   ```

## Routes and URLs

### Home and Static Pages
- **Home**: `/`
- **Test Page**: `/test/`
- **Thanks Page**: `/thanks/`

### User Authentication
- **Register**: `/accounts/signup/`
- **Login**: `/accounts/login/`
- **Logout**: `/accounts/logout/`

### Groups
- **List Groups**: `/groups/`
- **Create Group**: `/groups/create/`
- **Group Details**: `/groups/{group_id}/`

### Posts
- **List Posts**: `/posts/`
- **Create Post**: `/posts/create/`
- **Post Details**: `/posts/{post_id}/`
- **Delete Post**: `/posts/{post_id}/delete/`
- **User's Posts**: `/posts/user/{username}/`

## Project Structure
```
simplesocial/
│── accounts/            # User authentication (signup, login)
│── groups/              # Group management (create, join, browse)
│── posts/               # User posts (create, edit, delete)
│── templates/           # HTML templates for UI
│── static/              # CSS and JavaScript files
│── simplesocial/        # Project configuration
│── db.sqlite3           # SQLite database
│── manage.py            # Django management script
```

## Planned Improvements
- **Like & Comment System**: Users can like and comment on posts
- **Follow System**: Users can follow others
- **API Integration**: Convert functionalities to REST API for frontend use

## Author
Luc-b

