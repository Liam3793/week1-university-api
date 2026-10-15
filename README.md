# University API

A simple REST-based University API.

## Installing

Preferably in a Python virtual environment:

```bash
python -m pip install -r requirements.txt
```

## Running

```bash
uvicorn main:app --reload
```

## API

| Path | Summary |
|---|---|
| `/` | Return details about the overall API. |
| `/students/` | Return info for all students. |
| `/students/{student_id}` | Return info for the student with ID *student_id*. |