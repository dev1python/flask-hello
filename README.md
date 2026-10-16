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

## Docker image

The publish workflow builds this repository and pushes:

```text
yogenjadeja/flask-hello:1.0.0
```

The version comes from `version.txt`. On GitHub, the repository needs:

| Name | Kind | Value |
| --- | --- | --- |
| `DOCKERHUB_NAMESPACE` | Variable | `yogenjadeja` |
| `DOCKERHUB_USERNAME` | Secret | Docker Hub username |
| `DOCKERHUB_TOKEN` | Secret | Docker Hub access token |

Run the **Docker Publish** workflow manually, or merge a pull request into `main`.
