# Authentification-Flask

This is a simple user authentication system built using Flask, SQLAlchemy, and Flask-Login. Users can register, log in, log out, and access protected routes.

## Installation

1. Clone this repository to your local machine.
2. Navigate to the project directory.
3. Create a virtual environment: `python3 -m venv venv`.
4. Activate the virtual environment:
   - On Windows: `venv\Scripts\activate`
   - On macOS and Linux: `source venv/bin/activate`
5. Install dependencies: `pip install -r requirements.txt`.
6. Run the application: `python main.py`.

## Usage

### Register
- Access the registration page by visiting `/register`.
- Provide an email, name, and password.
- After successful registration, you will be automatically logged in.

### Login
- Access the login page by visiting `/login`.
- Enter your registered email and password.
- After successful login, you will be redirected to the secrets page.

### Secrets
- Access the secrets page by visiting `/secrets`.
- You need to be logged in to access this page.
- Displays the name of the logged-in user.

### Logout
- Click on the "Logout" link in the navigation bar to log out.
- You will be redirected to the home page after logging out.

### Download
- Access the download route by visiting `/download`.
- You need to be logged in to download the file.
- Serves a PDF file for download.

## Configuration

- You can change the secret key used for session management by modifying the `SECRET_KEY` variable in `app.py`.
- The database URI is set to a SQLite database named `users.db`. You can change this in `app.py` by modifying the `SQLALCHEMY_DATABASE_URI` variable.

## Credits

This project is inspired by various Flask tutorials and documentation.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
