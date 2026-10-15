University API
A simple REST-based University API.

Installing
Preferably in a Python venv: python -m pip install -r requirements.txt

Running
uvicorn main:app --reload
API
Path	Summary
/	Return details about the overall API.
/students	Return info for all students.
/students/<student-id>	Return info for the student with id student-id.