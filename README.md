# flask-hello

A small Flask app for trying a personal GitHub repository.

## Run

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

Open http://127.0.0.1:5000/

## Check

```bash
python -m unittest test_app.py
```

## Pages

| Path | Response |
| --- | --- |
| `/` | A short hello message |
| `/health` | `{"status": "ok"}` |
