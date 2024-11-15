\# AI Agent App

A web application where you can upload any PDF doc, use ChatGPT API, and answer questions related to it.

\------------------------------------

\------------------------------------

\*\*Pre-Project setup on Mac:

Install Homebrew first if you haven't:

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

Then install Python (includes pip):

brew install python

Verify installation on macOS/Linux:

pip3 --version

Upgrading pip (all platforms):

macOS/Linux:

pip3 install --upgrade pip

\------------------------------------

\------------------------------------

\*Step1: let's create the project directory structure:

\*\* Create project directory and subdirectories

mkdir pdf\_chat\_app

cd pdf\_chat\_app

mkdir templates uploads

touch app.py .env

\* Create a virtual environment and activate it

python3 -m venv venv

\* On macOS/Linux:

source venv/bin/activate

\* Install required packages
pip install --upgrade pip
python3 -m pip install flask PyPDF2 python-dotenv openai BeautifulSoup4 requests

\* Verify the installation
pip3 list | grep openai

\* If you get any errors, try:
python3 -m pip install --upgrade openai
or
pip3 install --upgrade openai

\* If you still have issues, try:
pip uninstall openai
pip install openai==0.28.1 # or the latest stable version


\------------------------------------

\*\*Step2, you'll need to get an OpenAI API key:

\*\*

Go to https://platform.openai.com/

Sign up or log in

Go to API Keys section

Create a new secret key

Copy the key (you won't be able to see it again)

\------------------------------------

\------------------------------------

\*\* Step3:Create the .env file:

\*\*

OPENAI\_API\_KEY=your\_api\_key\_here

\------------------------------------

\------------------------------------

\*\* Step4: Create the app.py file in your project directory:

\*\*

see the Python code in app.py

\------------------------------------

\------------------------------------

\*\* Step 6: Create index.html in the templates directory:

\*\*

See HTML code in templates/index.html

Your project structure should look like this:

Copypdf\_chat\_app/

├── venv/

├── app.py

├── .env

├── templates/

│ └── index.html

└── uploads/

\*\* Step7: Run the application:

\*\*

Make sure your virtual environment is activated

On macOS/Linux:

source venv/bin/activate

Run the Flask application

python3 app.py

\*\* Step8: Access the application:

\*\*

Go to http://127.0.0.1:5000

You should see the PDF Chat Application interface

To test the application:

Click "Choose File" and select a PDF document

Click "Upload"

Wait for the "File uploaded successfully" message

Type a question in the input field

Click "Ask" or press Enter

Wait for the response from the ChatGPT API
