# Set up

We'll need a few things to install for this section:
- behave (http://pythonhosted.org/behave/)
- selenium (http://selenium-python.readthedocs.io/installation.html)
- https://sites.google.com/a/chromium.org/chromedriver/downloads
# (my note)
- for Windows, the file ```chromedriver.exe``` has to be in the PATH, and it has to match the Chrome version
- Chrome has to be installed
## Running the tests

To run the tests, you'll need to do this in a terminal (but remember to have the Flask app running!):

```bash
pip install virtualenv
virtualenv venv --python=python3.9  # your version
source venv/bin/activate  # or venv\Scripts\activate.bat on Windows
cd section10
python -m behave tests\acceptance
```

If you want to run the tests in PyCharm, you'll need to create appropriate configurations. We cover this in the course!

# (my note)
- the ```app.py``` has to be running
in PyCharm (Windows), make 2 configurations for each app.py and Acceptance tests (locate behave.exe in \venv\Scripts)
run the tests from "Run/Debug" configuration (on the top-right in PyCharm)
- you can also run ```app.py``` from the command line manually instead
- i spent a lot of time debugging these tests because the course video code and the final_code.zip data don't match
perhaps due long time the video had been released
