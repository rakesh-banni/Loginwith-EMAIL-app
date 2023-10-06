# Loginwith-EMAIL-app
<h1>Django Website for User Authentication with Email Verification</h1>
* This Django project is a simple web application that provides user authentication functionality with email verification. It includes the following pages:

  ->   Sign Up: Users can register for a new account by providing their username, email address, and password. Upon successful registration, a verification link is sent to the provided email            address.

  ->   Email Verification: After signing up, users receive an email containing a verification link. Clicking the link verifies their email address and activates their account.

  ->   Sign In: Registered users can log in using their email and password.

  ->   Home Page: Once authenticated, users are redirected to the home page, which can be customized to suit the project's requirements.

* Features
  ->  User registration with email verification.<br>
  ->  Secure password storage using Django's built-in authentication system.<br>
  ->  User login with session management.<br>
  ->  Customizable home page for authenticated users.<br>
  ->  Built-in error handling and form validation.<br>
* Getting Started
  ->  Follow these steps to set up and run the project locally:

      Clone the Repository: Clone this repository to your local machine using git clone.

      Create a Virtual Environment: Create a Python virtual environment to isolate project dependencies.

      bash
      Copy code
      python -m venv venv
      Activate the Virtual Environment: Activate the virtual environment.

  -> On Windows:

      bash
      Copy code
      venv\Scripts\activate
  
  -> On macOS and Linux:
      
      bash
      Copy code
      source venv/bin/activate
      Install Dependencies: Install the required Python packages from the requirements.txt file.
      
      bash
      Copy code
      pip install -r requirements.txt
* Set Up Environment Variables: Create a .env file in the project's root directory and add your environment variables. You'll need to specify your email configuration for sending verification      emails. Here's an example .env file:

  makefile
  Copy code
  EMAIL_BACKEND=django.core.mail.backends.smtp.EmailBackend<br>
  EMAIL_HOST=your-smtp-host.<br>
  EMAIL_PORT=587<br>
  EMAIL_USE_TLS=True<br>
  EMAIL_HOST_USER=your-email@example.com<br>
  EMAIL_HOST_PASSWORD=your-email-password<br>
  SECRET_KEY=your-secret-key<br>
  DEBUG=True<br>
  Run Migrations: Apply the database migrations.<br>

  bash
  Copy code
  python manage.py migrate
  Create a Superuser: Create an admin superuser account to access the Django admin interface.
  
  bash
  Copy code
  python manage.py createsuperuser
  Run the Development Server: Start the development server.
  
  bash
  Copy code
  python manage.py runserver
* Access the Application: Open your web browser and go to http://localhost:8000 to access the project. You can sign up, sign in, and explore the home page.

* Project Structure
* The project's file structure follows Django's recommended layout:

  authentication/: The main Django app for user authentication and email verification.<br>
  templates/: Contains HTML templates for rendering pages.<br>
  static/: Stores static files such as CSS and JavaScript.<br>
  venv/: The Python virtual environment folder.<br>
  manage.py: Django's command-line utility for managing the project.<br>
  requirements.txt: Lists project dependencies.<br>
* Usage
  Feel free to use and customize this project for your authentication needs. You can enhance it further by adding additional features, such as user profiles, password reset functionality, or       user roles.
