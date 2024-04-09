## Introduction

This project consists of a series of tasks aimed at implementing internationalization (i18n) and localization (l10n) features using Flask and Babel extension. The tasks involve setting up a Flask application, integrating Babel for translation and localization, handling user locale preferences, inferring time zones, and displaying current time in different locales.

## Requirements

- All files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7)
- All files should end with a new line
- A README.md file, at the root of the folder of the project, is mandatory
- The code should use the pycodestyle style (version 2.5)
- The first line of all files should be exactly `#!/usr/bin/env python3`
- All *.py files should be executable
- All modules should have documentation (`python3 -c 'print(__import__("my_module").__doc__)'`)
- All classes should have documentation (`python3 -c 'print(__import__("my_module").MyClass.__doc__)'`)
- All functions and methods should have documentation (`python3 -c 'print(__import__("my_module").my_function.__doc__)'` and `python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'`)
- A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class, or method (the length of it will be verified)
- All functions and coroutines must be type-annotated.

## Tasks

### 0. Basic Flask app
Create a basic Flask app with a single route and an index.html template that outputs "Welcome to Holberton" as page title and "Hello world" as header.

### 1. Basic Babel setup
Install and configure the Babel Flask extension. Set up supported languages as ["en", "fr"].

### 2. Get locale from request
Create a function to determine the best match for the locale based on the request's accept languages.

### 3. Parametrize templates
Use gettext function to parametrize templates and provide translations for message IDs. Initialize translations and compile dictionaries.

### 4. Force locale with URL parameter
Implement a way to force a particular locale by passing the locale=fr parameter to the app’s URLs.

### 5. Mock logging in
Mock user login system by creating a user table and implementing a function to get user information. Display a welcome message if a user is logged in.

### 6. Use user locale
Change get_locale function to use a user’s preferred local if it is supported.

### 7. Infer appropriate time zone
Define a function to infer the appropriate time zone based on user settings or URL parameters.

### 8. Display the current time (Advanced)
Display the current time on the home page in the default format based on the inferred time zone.

## Usage

To run the Flask application for each task, execute the corresponding Python file (e.g., `python3 0-app.py`) after ensuring all dependencies are installed.

## Author

Yabs Mullo
