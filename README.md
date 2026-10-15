# Web Data Extractor

Web Data Extractor is a lightweight FastAPI application for scraping structured data from web pages and storing results in SQLite. It includes a CLI for running jobs locally and a test suite for validating the scraper and API.

## Features
- FastAPI REST API
- SQLite storage using SQLModel
- CLI-based scraping jobs via Typer
- Background processing for scrape jobs
- Docker support
- GitHub Actions CI
- MIT license

## Tech Stack
- Python 3.11
- FastAPI
- SQLModel
- Typer
- BeautifulSoup
- SQLite
- Pytest

## Project Structure
- `app/main.py` – FastAPI app
- `app/db.py` – database setup and session management
- `app/models.py` – SQLModel database models
- `app/schemas.py` – request/response schemas
- `app/scraper.py` – scraping logic
- `cli.py` – CLI entrypoint
- `tests/` – test suite
- `Dockerfile` – container build
- `docker-compose.yml` – container orchestration
- `.github/workflows/ci.yml` – CI workflow

## Quickstart

### 1) Create and activate virtual environment
```bash
python -m venv .venv
source .venv/bin/activate
