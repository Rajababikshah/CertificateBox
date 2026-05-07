# Byte-Block Secure Digital Certificate Locker (BBSDCL)

## Project Overview
A Flask-based web application for secure digital certificate management.

## How to Run Locally
1. Install Python 3.7+
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Configure environment variables (optional but recommended):
  - Copy `.env.example` to `.env` and fill in your DB settings, OR
  - Export env vars in your shell (e.g. `DATABASE_URL`)
4. Run the app:
   ```
   python main.py
   ```

## Deployment (e.g., Render.com)
- **Build Command:**
  ```
  pip install -r requirements.txt
  ```
- **Start Command:**
  ```
  gunicorn main:app
  ```

## Database Configuration (MySQL)
This app expects a MySQL database. Configure **one** of the following:

- **Option A (recommended):** `DATABASE_URL` in the form `mysql://USER:PASSWORD@HOST:PORT/DBNAME`
- **Option B:** individual env vars (Railway-style or generic):
  - `MYSQLHOST` or `DB_HOST`
  - `MYSQLPORT` or `DB_PORT`
  - `MYSQLUSER` or `DB_USER`
  - `MYSQLPASSWORD` or `DB_PASSWORD`
  - `MYSQLDATABASE` (or `MYSQL_DATABASE`) or `DB_NAME`

Note: the app now connects to MySQL lazily (on first DB usage) so the web server can boot even if the DB is temporarily unavailable.

## Project Structure
- `main.py` — Main Flask app
- `static/` — Static files (CSS, JS, images)
- `templates/` — HTML templates
- `database/` — SQL files

## License
Specify your license here.
