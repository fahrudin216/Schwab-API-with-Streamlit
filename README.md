# Schwab API with Streamlit

Interactive Streamlit app for Charles Schwab market data workflows — option chains, price history charts, and account views.

## Features

- Password-protected Streamlit multipage app
- Option chain search examples
- Price history charts
- Account information views
- Built on `schwabdev` + Streamlit

## Stack

`Python` · `Streamlit` · `schwabdev` · `requests`

## Setup

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

Create `.streamlit/secrets.toml`:

```toml
password = "your-local-password"
```

Configure Schwab API credentials as required by `schwabdev` (do not commit secrets).

## Run

```bash
streamlit run app.py
```

## Project layout

```text
app.py          Streamlit entry + auth pages
src/            API / data helpers
ui/             UI page modules
.streamlit/     Streamlit config (local secrets)
```

## Notes

- Keep credentials and tokens out of git
- For educational / personal tooling — not financial advice

Related: [Schwab-Market-Analysis](https://github.com/fahrudin216/Schwab-Market-Analysis)
