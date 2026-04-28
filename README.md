# Byte-Block Secure Digital Certificate Locker (BBSDCL)

## Project Overview
A Flask-based web application for secure digital certificate management.

## How to Run Locally
1. Install Python 3.7+
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Run the app:
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

## Project Structure
- `main.py` — Main Flask app
- `static/` — Static files (CSS, JS, images)
- `templates/` — HTML templates
- `database/` — SQL files

## License
Specify your license here.
