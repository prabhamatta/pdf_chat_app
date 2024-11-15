# PDF Chat App
 A web application where you can upload any PDF doc, use ChatGPT API, and answer questions related to it.
 
------------------------------------
------------------------------------

Pre-Project setup on Mac:
# Install Homebrew first if you haven't:
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Then install Python (includes pip):
brew install python

# Verify installation on macOS/Linux:
pip3 --version

# Upgrading pip (all platforms):
# macOS/Linux:
pip3 install --upgrade pip



------------------------------------
------------------------------------



**Step1: let's create the project directory structure:
# Create project directory and subdirectories
mkdir pdf_chat_app
cd pdf_chat_app
mkdir templates uploads
touch app.py .env

# Create a virtual environment and activate it
python3 -m venv venv

# On macOS/Linux:
source venv/bin/activate

# Install required packages
pip3 install flask PyPDF2 python-dotenv openai

------------------------------------
------------------------------------

**Step2, you'll need to get an OpenAI API key:


Go to https://platform.openai.com/
Sign up or log in
Go to API Keys section
Create a new secret key
Copy the key (you won't be able to see it again)

------------------------------------
------------------------------------

**Step3:Create the .env file:

OPENAI_API_KEY=your_api_key_here
------------------------------------
------------------------------------


**Step4: Create the app.py file in your project directory:

see the Python code in app.py

------------------------------------
------------------------------------

**Step 6: Create index.html in the templates directory:


See HTML code in templates/index.html


Your project structure should look like this:

Copypdf_chat_app/
├── venv/
├── app.py
├── .env
├── templates/
│   └── index.html
└── uploads/

**Step7: Run the application:

# Make sure your virtual environment is activated
# On macOS/Linux:
source venv/bin/activate

# Run the Flask application
python3 app.py

**Step8: Access the application:


** Step8: Open your web browser
Go to http://127.0.0.1:5000
You should see the PDF Chat Application interface

To test the application:

Click "Choose File" and select a PDF document
Click "Upload"
Wait for the "File uploaded successfully" message
Type a question in the input field
Click "Ask" or press Enter
Wait for the response from the ChatGPT API


