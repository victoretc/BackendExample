# BackendExample

To write a simple API in Flask, you can follow these steps:

1. Install Flask: First, you need to install the Flask library. You can do this by running the following command:
MacOS
```bash
pip3 install Flask.
```

2. Create a Python file: Create a new Python file in your project directory. This file will contain your Flask API code.

3. Import Flask: In your Python file, import the Flask library by adding the following line of code at the top:
```python
from flask import Flask.
```

Create a Flask app instance: Create a new instance of the Flask class by adding the following code to your Python file:

```python
app = Flask(__name__)
```
This will create a new Flask application instance.

Define a route: Define a route for your API by adding the following code:
```python
@app.route('/')
def hello():
    return 'Hello, World!'
```
This code defines a route at the root URL ('/') and returns the string 'Hello, World!' when the route is accessed.

```python
if __name__ == '__main__':
    app.run()
```

To run a Flask app, you need to follow these steps:

Set the environment variables: Flask requires the FLASK_APP environment variable to be set to the name of the Python file that contains the Flask app. You can set this variable by running the following command in the terminal:

```bash
export FLASK_APP=main.py
```
Create and activate the virtual environment (optional): If you are using a virtual environment, you need to activate it before running the Flask app. You can activate the virtual environment by running the following command:

MacOS
```bash
python3 -m venv venv
source venv/bin/activate
```

Install requirements.txt file

MacOs
```bash
pip3 install -r requirements.txt
```

Run the Flask app: Once the environment variables are set, you can run the Flask app by running the following command in the terminal:
flask run

This command will start the Flask app and make it available at http://127.0.0.1:5000/ in your web browser.

If you want to run the Flask app on a specific IP address or port, you can pass the --host and --port options to the flask run command. For example:

```bash
flask run --host=0.0.0.0 --port=8080
```
This command will start the Flask app on all available network interfaces (0.0.0.0) and port 8080.

Overall, running a Flask app is a simple process that involves setting environment variables and running the Flask app using the flask run command.