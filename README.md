**Python CI Pipeline with GitHub Actions**

📌 Project Overview
This project implements a Continuous Integration (CI) workflow for a Python application using GitHub Actions.
The pipeline runs automated tests, generates code coverage reports, checks code style and complexity, and uploads the source code as an artifact.
It is triggered on pushes and pull requests to the main and develop branches.

**🛠 Tech Stack**
    - Python (configurable via matrix or environment variable)
    
    - pytest – running unit tests
    
    - coverage – generating test coverage reports
    
    - flake8 – linting and complexity checks
    
    - GitHub Actions – CI automation

**🚀 What Was Done**
1. Created a python-ci job that:

    - Runs unit tests using pytest.
    
    - Generates a coverage report with coverage.
    
    - Checks code style with flake8.
    
    - Checks code complexity with flake8.
    
    - Prints the coverage report in the console.

2. Configured artifact upload to store the Python source code.

3. Set up triggers for workflow execution:

    - Push to main and develop branches.
    
    - Pull request to main.

4. Customized the workflow run name to include:

    - GitHub username of the person who triggered the job.
    
    - Commit hash that triggered the workflow.
