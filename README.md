SECURE PASSWORD MANAGER

This is a secure password manager built with python, SQLite, Flask and cryptograghy library. it is web based and 
its fucntions are, it allows users to register, generate secure passwords, store website credentials securely and modify heir stored credentials.

FEATURES

1) very secure password generation
2) hashing passwords with werkzeug
3) registering users
4) user log in and log out
5) modfidication of stored credentials
6) CSRF Protection with Flask-WTF
7) protection against SQL injection by using parameterised queries
8) basic XSS protection through jinja escaping

PROJECT STRUCTURE

1) app.py
2) config.py
3) database.py
4) security.py
5) requirements.txt
6) template/
7) static/

   
HOW TO RUN

1) ensure that requirements.txt is installed, if not, do this
"py -m pip install -r requirements.txt"

2) The project uses a .env file to store the Flask secret key. so, before running the project, in the same folder as the app.py, create a .env file and 
enure the secret key is added.
to create a secure key, run this on your terminal, "py -c "import secrets; print(secrets.token_hex(32))" ".
inside the .env file, add this "SECRET_KY=secrete_key_generated_from_the_command".

So the .env file is not uploaded on github because it has private configuartion data that shoudln't be easily accessed

now run app.py, after running, the app will generate a link "http://127.0.0.1:5000".
open the link on a web browser.

then you can now perform the several fucntions of the project.
1) register
2) log in
3) store credentials
4) edit your stored credentials
5) delete credentials
6) log out







