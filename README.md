FastAPI API Automation with CI/CD

Overview

This repository demonstrates how to set up a FastAPI backend, automate API testing using pytest, and integrate the tests into a GitHub Actions CI/CD pipeline. The project covers fundamental DevOps practices such as continuous testing, test automation, and CI/CD workflow implementation.

Features

FastAPI backend with basic mathematical operations (add, subtract, multiply)

Automated API testing using Python's requests library and pytest

CI/CD integration using GitHub Actions for automated testing on code changes

Configurable GitHub Actions workflow for automated test execution

Prerequisites

Ensure you have the following installed:

Python 3.10+

FastAPI

Uvicorn

Requests

Pytest

Installation

1. Clone the repository

 git clone https://github.com/your-username/your-repo.git
 cd your-repo

2. Install dependencies

 pip install -r requirements.txt

Running the FastAPI Server

Start the FastAPI server with the following command:

 python app.py

The server will be available at http://localhost:8000

API Endpoints

GET / - Returns a simple welcome message.

GET /add/{num1}/{num2} - Adds two numbers and returns the result.

GET /subtract/{num1}/{num2} - Subtracts two numbers and returns the result.

GET /multiply/{num1}/{num2} - Multiplies two numbers and returns the result.

Running Tests

1. Run basic API tests

 python test_pytests.py

2. Run tests using pytest

 pytest test_pytests.py

GitHub Actions Integration

This repository includes a GitHub Actions workflow (.github/workflows/test.yml) that automates testing on every push or pull request to the main branch.

Steps in the Workflow:

Checkout the repository

Set up Python environment

Install dependencies

Start the FastAPI server

Run API tests using pytest

Setting up GitHub Actions

Push the changes to GitHub to trigger the CI/CD pipeline:

git add .
git commit -m "Add test automation and GitHub Actions"
git push origin main

You can monitor the test execution under the Actions tab in your GitHub repository.

Future Enhancements

Implement database integration (PostgreSQL/MongoDB)

Add authentication and authorization mechanisms

Enhance logging and error handling

Perform performance and load testing using locust.io
