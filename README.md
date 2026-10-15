University API

A simple University API built using Python and FastAPI for Week 1 Homework.

Get information about the University API.

Get a list of all students.

Get information about a specific student using their ID.

Return a 404 error if a student cannot be found.

TECHNOLOGIES USED

Python
FastAPI
Uvicorn

PROJECT STRUCTURE 

week1-university-api/
├── main.py
├── requirements.txt
├── routers/
│   ├── __init__.py
│   └── students.py
└── README.md

HOW TO RUN THE PROJECT

1) eate a virtual environment:

python3 -m venv .venv

2) Activate the virtual environment on macOS:

source .venv/bin/activate

3) Install the required packages:

python -m pip install -r requirements.txt

Start the API server:

uvicorn main:app --reload

4) Open your browser and visit:

http://127.0.0.1:8000

API Endpoints

Method

Endpoint

Description

GET

/

API information

GET

/students/

Get all students

GET

/students/s1

Get student s1

GET

/students/s2

Get student s2

GET

/students/s3

Get student s3

GET

/students/s10

Returns 404 because the student does not exist

Error Handling

If a student ID does not exist, the API returns HTTP status code 404 and the following JSON:

{
  "detail": "Student not found"
}

Author

Liam3793

Purpose

Created as part of the Week 1 University API homework exercise.