# Back-end

This folder includes the data itself, and a simple API built on [FastAPI](https://fastapi.tiangolo.com/) to serve it. You will need `python 3.11`

## Testing Locally
1. Clone the repository.
2. Navigate to the `Server/FastAPI (Data)` directory.
3. Set up virtual environment with `python3.11 -m venv venv`.
4. Activate environment with `source venv/bin/activate`.
5. Install requirements with `pip install -r reqs.txt`.
6. Run the app through uvicorn with `uvicorn main:app --reload`.

## Running Remotely
You will need something for process control, such as [Supervisor](https://supervisord.org/). Afterwards, you can use `gunicorn` to run the server through the process.