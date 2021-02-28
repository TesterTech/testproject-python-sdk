# testproject-python-sdk
Code for the Youtube video https://youtu.be/CxS5SX8f4yQ

* Getting started with Python SDK for testproject.io
** On https://testproject.io
- [ ] First create an account 
- [ ] Login to that account 
- [ ] Go to the link and setup the developer token: https://app.testproject.io/#/integrations/sdk
- [ ] Copy the token to the clipboard
** Setup the DEV token
- For Linux and Mac
TP_DEV_TOKEN in your .bashrc or .bash_profile 
For example on Linux: export TP_DEV_TOKEN=<your dev token here>
- For Windows
Create env. variable TP_DEV_TOKEN in system settings and put the value there.
** Setup and connect to agent
- Visit testproject and click the agents menu (https://app.testproject.io/#/agents), select appropriate agent
- Download and install
- Once installer closes click on the message saying that the agent is not authorized
- You have to log into testproject.io (allow the popup if needed) all should be well
** Local computer
The example code and required dependencies are in the repository 
- Make sure you have python installed (python 3)
- sudo dnf install -y git  python3 
- pip3 install --user pipenv
- installed Google Chrome using RPM [https://www.google.com/chrome/] (restart agent)
  - Note that because this video is based on RPM based distro I install it using RPM package. Pick the package for your OS here.
- Clone the following github repository (git clone) https://github.com/testproject-io/python-sdk
- Navigate into that dir (cd python-sdk)
- pipenv install
- pipenv shell 
From within this virtual environment (python-sdk) install the Python sdk: 
- pip3 install testproject-python-sdk
Now run the test using python:
python tests/examples/simple/web_test.py
** Report
- For the report part, visit this link: https://docs.testproject.io/testproject-sdk/opensdk-v2/python-sdk#explicit-project-and-job-names
- Please note that if you provide a project that does not exist it will be created through SDK... BUT will not be accessible in testproject.io 
- Click the monitor tab and see the run. 

References
- Link to blogpost about this subject created by Bas Dijkstra, I basically extended this information in this video https://blog.testproject.io/2020/07/15/getting-started-with-testproject-python-sdk/
- SDK (inside your profile page on testproject.io) https://app.testproject.io/#/integrations/sdk
- Agents https://app.testproject.io/#/agents
- Github sample https://github.com/testproject-io/python-sdk
- Reporting and report names https://docs.testproject.io/testproject-sdk/opensdk-v2/python-sdk#explicit-project-and-job-names
- Download Google Chrome https://www.google.com/chrome/
  
