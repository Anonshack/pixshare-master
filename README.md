---

### Testing
 - `docker compose exec web python manage.py test`
 - `coverage run -m pytest`
 - Nox (includes sessions for black, lint, audit, tests)
     - testing supported for Python 3.11, 3.12, 3.13
     - e.g. `nox`, `nox -rs lint-3.13`, `nox -s tests`
       - `nox`
       - `nox -s black-3.12`
       - `nox -s docs-3.13`
       - `nox -rs lint-3.12` (Use the 'r' flag to reuse existing session)
       - `nox -s pyright-3.11`
       - `nox -s audit` (will run tests against all Python versions)
       - `nox -s tests`

---

