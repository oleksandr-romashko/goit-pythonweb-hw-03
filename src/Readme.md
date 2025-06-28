# goit-pythonweb-hw-03

A simple Flask web app with form handling, routing, and Jinja2 templates — part of GoIT FullStack Python homework #3.

## Features

- Routes: `/`, `/message`, `/read`
- Static assets: logo and styles
- Form submission with data saved to `storage/data.json`
- Custom 404 page
- Docker support (optional)

## Requirements

- Python 3.10+
- Poetry
- Flask

## Setup

```bash
poetry install
poetry run python src/main.py
```

App runs at: http://localhost:3000# goit-pythonweb-hw-03

A simple Flask web app with form handling, routing, and Jinja2 templates — part of GoIT FullStack Python homework #3.

## Features

- Routes: `/`, `/message`, `/read`
- Static assets: logo and styles
- Form submission with data saved to `storage/data.json`
- Custom 404 page
- Docker support (optional)

## Requirements

- Python 3.10+
- Poetry
- Flask

## Setup

```bash
poetry install
poetry run python src/main.py
```

## Run 

App runs at: http://localhost:3000

## Docker

docker build -t goit-pythonweb-hw-03 .
docker run -p 3000:3000 -v "$PWD/src/storage:/app/storage" goit-pythonweb-hw-03

## Project Structure

.
├── compose.yaml
├── Dockerfile
├── .dockerignore
├── pyproject.toml
└── src/
    ├── main.py
    ├── Readme.md
    ├── decorators/
    │   └── handle_server_errors.py
    ├── static/
    │   ├── images/
    │   │   └── logo.png
    │   ├── pages/
    │   │   ├── index.html
    │   │   └── message.html
    │   ├── scripts/ (placeholder)
    │   ├── styles/
    │   │   └── style.css
    │   └── templates/
    │       ├── error.html
    │       └── read.html
    └── storage/
    │   └── data.json
    └── utils/
        ├── constants.py
        └── validations.py

## Author

Oleksandr Romashko
alex.rmshk@gmail.com
MIT License