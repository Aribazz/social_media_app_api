# 1. Accomplishments So Far
- **User Management**: Created user registration, login, and profile management using Django's built-in auth system.
- **Posts Module**: Users can create, edit, delete, and list their posts.
- **Notifications**: Integrated a simple notification system for key events (e.g., new followers or post likes).
- **Database Setup**:
  - Currently using **SQLite** in development.
  - **PostgreSQL** installed but **not yet fully configured** for production.
- **API Development**:
  - RESTful endpoints implemented using **Django REST Framework (DRF)**.
  - Includes pagination, filtering, and token authentication.
- **Environment Configuration**:
  - Created a `.env` file for sensitive settings.
  - Introduced `django-environ` for environment-based configuration.
- **Initial Deployment Steps**:
  - Preparing production settings (allowed hosts, secret keys, static files).
- **Virtual Environment Setup**:
  - Used `venv` to isolate dependencies and Python packages.

# 2. Challenges Faced and Solutions
- Missing Dependencies: Faced errors due to missing libraries (e.g., `rest_framework`, `dj_database_url`).
  - *Solution*: Reviewed `requirements.txt` and reinstalled necessary packages using `pip install -r requirements.txt`.
- Environment Variables Not Recognized**: Encountered issues with setting up `.env` variables.
  - *Solution*: Installed `django-environ`, updated `settings.py` to load environment variables properly, and ensured `.env` was correctly formatted.
- Virtual Environment Activation Issues:
  - *Solution*: Reinstalled the virtual environment, activated it properly using `source .venv/bin/activate` (for Unix) or `.venv\Scripts\activate` (for Windows).
- ModuleNotFoundError for Django: Encountered issues running `python manage.py runserver`.
  - *Solution*: Verified Django installation inside the virtual environment and ensured correct Python interpreter selection in VS Code.

## 3. What’s Next? – Weekly Roadmap

- **✅ Finalize PostgreSQL Configuration**:
  - Update `DATABASES` in `settings.py`
  - Use `psycopg2` as the DB adapter
- **✅ Deployment**:
  - Choose hosting platform: Heroku, Render, DigitalOcean, or AWS
  - Set up production settings
- **🔍 Testing & Debugging**:
  - Add unit tests using Django’s test suite
  - Check for edge cases in API calls
- **📊 Performance Optimization**:
  - Use `select_related()` and `prefetch_related()` in queries
  - Add caching (e.g., Redis)
- **📚 Documentation**:
  - Auto-generate docs with Swagger or Postman
  - Write clear endpoint usage instructions for frontend devs
- **📦 API Versioning**:
  - Plan for `/api/v1/` structure in future updates

---

## 🛠️ Tech Stack

- **Backend**: Python, Django, Django REST Framework
- **Database**: SQLite (dev), PostgreSQL (prod - in progress)
- **Authentication**: Token-based (DRF’s TokenAuth)
- **Environment Management**: `python-dotenv`, `django-environ`
- **Virtual Environment**: `venv`
- **Deployment (upcoming)**: Heroku / DigitalOcean / Render

---

## ⚙️ Environment Setup

### 4. Clone the Repo

```bash
git clone https://github.com/yourusername/social_media_api.git
cd social_media_api

