# DevNDesign (DND)

### Freelancing marketplace for developers, designers, and clients

[![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?logo=php&logoColor=white)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-8-4479A1?logo=mysql&logoColor=white)](https://www.mysql.com/)
[![HTML5](https://img.shields.io/badge/Frontend-HTML%2FCSS%2FJS-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> Post projects, apply as a freelancer, collaborate with file exchange — a classic marketplace product built as a full PHP/MySQL web app with role-based access and hardened auth.

Built by **[veera](https://github.com/veera-1175)**.

---

## Product overview

**DevNDesign** connects two sides of freelance work:

| Role | What they can do |
|------|------------------|
| **Client** | Register, post jobs, review applicants, manage projects |
| **Freelancer** | Browse / filter jobs, apply, exchange files, track work |

The system is designed for **simplicity and trust**: session auth, hashed passwords, prepared statements, and responsive pages that work on desktop and mobile.

---

## Features

- Registration & login with secure password hashing
- Role-based access (Client / Freelancer)
- Job posting and applications
- Search & filtering for projects
- File upload / download for collaboration
- Session-based authentication
- Responsive UI across devices

---

## Security

| Practice | Implementation |
|----------|----------------|
| Password storage | `password_hash()` / `password_verify()` |
| SQL injection | Prepared statements |
| Access control | Session + role checks on protected pages |
| Sessions | Server-side session management |

---

## Tech stack

| Layer | Tech |
|-------|------|
| Frontend | HTML, CSS, JavaScript |
| Backend | PHP |
| Database | MySQL |
| Local runtime | Apache (XAMPP / similar) |

---

## Quick start

```bash
git clone https://github.com/veera-1175/DND-DevNDesign.git
```

1. Copy the project into your Apache document root (e.g. `xampp/htdocs/DND-DevNDesign`).
2. Start **Apache** and **MySQL**.
3. Create the database and import the provided SQL schema (see `database/` or `*.sql` in the repo).
4. Update DB credentials in the PHP config / connection file.
5. Open `http://localhost/DND-DevNDesign` (path depends on your folder name).

---

## Project layout

```
DND-DevNDesign/
├── *.php                 # Pages & handlers
├── css / js / assets     # Frontend
├── uploads/              # Shared files (gitignored if present)
├── database/ or *.sql    # Schema
└── README.md
```

---

## Interview walkthrough

| Topic | Talking point |
|-------|----------------|
| Domain | Two-sided marketplace — clients hire, freelancers apply |
| Backend fundamentals | PHP sessions, CRUD, file I/O, MySQL |
| Security | Hashing, prepared statements, RBAC |
| UX | Role-aware navigation and responsive layouts |

**Demo path:** register client → post job → register freelancer → apply → show file exchange.

---

## License

MIT © [veera](https://github.com/veera-1175)

**DevNDesign** — hire talent, ship projects.
