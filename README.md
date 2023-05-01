# BackendExample

To write a simple API in Flask, you can follow these steps:

Install Flask: First, you need to install the Flask library. You can do this by running the following command:
For mac 
pip3 install Flask.

Create a Python file: Create a new Python file in your project directory. This file will contain your Flask API code.

Import Flask: In your Python file, import the Flask library by adding the following line of code at the top: from flask import Flask.

Create a Flask app instance: Create a new instance of the Flask class by adding the following code to your Python file:


app = Flask(__name__)
This will create a new Flask application instance.

Define a route: Define a route for your API by adding the following code:

@app.route('/')
def hello():
    return 'Hello, World!'
This code defines a route at the root URL ('/') and returns the string 'Hello, World!' when the route is accessed.

Run the app: Finally, run the Flask app by adding the following code:
Copy
if __name__ == '__main__':
    app.run()

This will start the Flask app and make it available at http://localhost:5000/ in your web browser.

Here is the complete code for a simple Flask API that returns a "Hello, World!" message
You can add more routes and functionality to your Flask API as needed.


To run a Flask app, you need to follow these steps:

Set the environment variables: Flask requires the FLASK_APP environment variable to be set to the name of the Python file that contains the Flask app. You can set this variable by running the following command in the terminal:
export FLASK_APP=main.py

Create and activate the virtual environment (optional): If you are using a virtual environment, you need to activate it before running the Flask app. You can activate the virtual environment by running the following command:

For MAC
```bash
python3 -m venv venv
source venv/bin/activate
```

Install requirements.txt file
For MAC
pip3 install -r requirements.txt

Run the Flask app: Once the environment variables are set, you can run the Flask app by running the following command in the terminal:
flask run

This command will start the Flask app and make it available at http://127.0.0.1:5000/ in your web browser.

If you want to run the Flask app on a specific IP address or port, you can pass the --host and --port options to the flask run command. For example:

flask run --host=0.0.0.0 --port=8080
This command will start the Flask app on all available network interfaces (0.0.0.0) and port 8080.

Overall, running a Flask app is a simple process that involves setting environment variables and running the Flask app using the flask run command.