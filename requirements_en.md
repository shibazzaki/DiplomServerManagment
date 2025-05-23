# 📋 **Requirements for the Web Application for Automated Game Server Management**

## ✅ **1. Functional Requirements**

1.1 Start, stop, and restart game servers via web interface or API
1.2 Retrieve server status (running / stopped / error)
1.3 Collect and display statistics (uptime, resource usage)
1.4 Log server launches, crashes, and user actions
1.5 Manage multiple servers simultaneously (scalable structure)
1.6 Provide an API for integration with third-party tools (e.g., Telegram bots)
1.7 View logs in the web interface
1.8 Enable automatic restarts or scheduled maintenance (future integration with cron/task queue)

---

## 💎 **2. Non-Functional Requirements**

2.1 Operates on any Ubuntu-based Linux system
2.2 Easy deployment via a single `docker-compose up --build` command
2.3 Scalable architecture allowing new servers to be added via configuration
2.4 Minimal dependencies: Python, Docker, PostgreSQL, Linux shell
2.5 Environment variables and configuration stored in `.env`
2.6 Support for headless operation (API-only mode)

---

## 🧪 **3. Technical Requirements**

### 🔸 Infrastructure:

* Linux (Ubuntu/KDE Neon or compatible)
* Docker, Docker Compose

### 🔸 Backend:

* Python 3.12+
* Flask framework
* SQLAlchemy ORM
* PostgreSQL
* `python-dotenv` for environment config

### 🔸 Frontend:

* HTML5 + Bootstrap 5
* JavaScript (Vanilla or Axios)

### 🔸 Monitoring:

* `psutil` library (CPU, RAM, disk metrics)
* `tmux` for running background server processes

### 🔸 Documentation:

* Swagger / OpenAPI specification (e.g., via Flask-RESTX)
* Markdown for technical and user documentation

---

## 🛡️ **4. Security Requirements**

* API access restricted to authenticated users (via API tokens or access keys)
* Log files are read-only and protected from unauthorized edits
* Role-based access control (admin / user separation planned)
* Resource limits applied to Docker containers running game servers

---

## 🎯 **5. Quality Requirements**

* High modularity of codebase: separate API, monitoring logic, and data layers
* Unit tests for core components using `pytest`
* Input validation for API parameters (e.g., server commands)
* Optional database backup mechanisms
* Codebase adheres to PEP8 style guide; formatting via `black`, linting via `pre-commit`

---

Готовий рухатися далі? Можемо продовжити з моделюванням бази чи Flask-API.
