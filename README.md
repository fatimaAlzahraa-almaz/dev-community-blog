**Project**

- **Name**: Dev Community Blog — a development-focused community platform for developers to share posts, comment, and interact.

**Description**

- **Overview**: This repository contains a full-stack web application: a Django REST Framework backend and a Next.js frontend. The platform supports user accounts, posts, bookmarks, likes, comments, follows, and other developer-community interactions.

**Features**

- **User Accounts**: registration, login, profiles, and follow system.
- **Posts**: create, edit, delete, image support, and slug-based post pages.
- **Interactions**: likes, bookmarks, comments, and follows.
- **Search & Filters**: search posts and filter by categories/tags.

**Architecture**

- **Backend**: Django + Django REST Framework (APIs, authentication, permissions).
- **Frontend**: Next.js (React) with server/client components for the UI and state management.
- **Folder Layout**: Backend code lives in the `backend/` folder and frontend code lives in the `frontend/` folder.

**Tech Stack**

- **Backend**: Python, Django, Django REST Framework. See [backend/manage.py](backend/manage.py#L1).
- **Frontend**: TypeScript, Next.js. See [frontend/package.json](frontend/package.json#L1).

**Getting Started (Development)**

- **Prerequisites**: Python 3.10+, Node.js 18+, and either `pipenv` (recommended for backend) or `venv` + `pip`.

**Backend (local)**

- **Install dependencies**: `pipenv install --dev` (or `pip install -r requirements.txt` if using a requirements file).
- **Environment**: create `.env` (or set env vars) for `DJANGO_SECRET_KEY`, `DATABASE_URL`, and any other needed settings.
- **Migrate DB**: `pipenv run python backend/manage.py migrate`.
- **Create superuser**: `pipenv run python backend/manage.py createsuperuser`.
- **Run server**: `pipenv run python backend/manage.py runserver`.

**Frontend (local)**

- **Install dependencies**: from the `frontend/` folder run `npm install` or `pnpm install`.
- **Configure API URL**: ensure the frontend points to the running backend API (e.g., `http://localhost:8000`). Update env vars in `frontend/.env.local` if present.
- **Run dev server**: `npm run dev` (from `frontend/`).

**Running Tests**

- **Backend tests**: `pipenv run python backend/manage.py test`.
- **Frontend tests**: run whichever test runner is configured (check `frontend/package.json`).

**APIs**

- The backend exposes REST endpoints using Django REST Framework. Browse the API or admin at `/admin` when the server is running.

**Contributing**

- **Code style**: follow existing project conventions.
- **Pull requests**: open feature branches and include tests for new behavior.
- **Issues**: open issues for bugs or enhancement requests.

**Deployment**

- Deploy backend to a suitable host (Heroku, Digital Ocean, AWS, etc.) and frontend to Vercel or another static/SSR host. Configure production environment variables and static/media storage.

**License**

- **License**: This project is offered under the MIT License (or choose your preferred license).

**Contact**

- **Maintainer**: Project maintainer — open an issue or pull request for questions and contributions.

**Files of Interest**

- **Backend entrypoint**: [backend/manage.py](backend/manage.py#L1)
- **Frontend entrypoint**: [frontend/src/app/page.tsx](frontend/src/app/page.tsx#L1)

Thanks for checking out the Dev Community Blog — happy building!
