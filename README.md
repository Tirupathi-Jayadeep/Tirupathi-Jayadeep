<div align="left">

# Tirupathi Jayadeep
**Backend Software Engineer & AI/ML Undergraduate** · Chennai, India  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/<your-linkedin-handle>)
[![LeetCode](https://img.shields.io/badge/LeetCode_200+-FFA116?style=flat-square&logo=leetcode&logoColor=black)](https://leetcode.com/u/<your-leetcode-handle>)
[![Email](https://img.shields.io/badge/tirupathijayadeep%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:tirupathijayadeep@gmail.com)

</div>

---

### About Me

I design **concurrency-safe backend systems**, **RESTful APIs**, and **constraint-optimization engines**. Currently pursuing a B.Tech in Artificial Intelligence & Machine Learning at **Saveetha Engineering College** (CGPA: `8.62`, Class of `2027`), I focus on turning messy operational workflows into deterministic, well-tested Python & PostgreSQL services.

- **Core Focus:** High-integrity relational schemas, row/advisory locking, RBAC architectures, and combinatorial optimization (CP-SAT / MILP).
- **Currently Exploring:** Distributed task queues, query-plan optimization in PostgreSQL, and container orchestration with Docker Compose.
- **Off the Clock:** Competitive chess player — applying look-ahead search and state-space pruning to both 64 squares and system architecture.

---

### Engineering Stack

| Domain | Technologies & Practices |
| :--- | :--- |
| **Backend & APIs** | `Python` · `Django` · `Django REST Framework (DRF)` · `RESTful Design` · `Session Auth` · `RBAC` |
| **Databases & Locking** | `PostgreSQL` (Advisory Locks, Row-Level Locking) · `MySQL` · `SQLite` · `Query Optimization` |
| **Optimization & Scientific** | `Google OR-Tools (CP-SAT)` · `SciPy (Hungarian Algorithm)` · `Algorithmic Benchmarking` |
| **Testing & DevOps** | `Pytest` (Automated API & Solver Suites) · `Docker` · `Docker Compose` · `Git` · `GitHub` |
| **CS Fundamentals** | `Data Structures & Algorithms (200+ LeetCode)` · `OOP` · `ACID & Concurrency Control` |

---

### Featured Systems

#### 1. [Bench Zero](https://github.com/tirupathijayadeep/bench-zero) — Constraint-Based Workforce Allocation Engine
> **Status:** Active / Production-Ready Containerized Build · **Role:** Sole Architect & Developer

* **Purpose:** Solves multi-constraint developer-to-project staffing while decoupling algorithmic recommendations from confirmed bookings via a human-in-the-loop approval pipeline.
* **Tech Stack:** `Python` · `Django` · `DRF` · `PostgreSQL` · `Google OR-Tools (CP-SAT)` · `SciPy` · `Docker`
* **Key Engineering Contributions:**
  * Formulated staffing as a Constraint Satisfaction / Integer Programming model in **OR-Tools CP-SAT**, benchmarking against a **SciPy Hungarian** baseline and a **Greedy** heuristic (**+5–12% allocation quality improvement** over greedy).
  * Eliminated race conditions during concurrent bulk-accept operations using **PostgreSQL advisory locks** and `select_for_update()` row-level locking alongside rate-limited DRF endpoints.
  * Built a complete audit trail for manager review/accept/reject actions and authored **57 automated `pytest` tests** covering solver correctness, RBAC permissions, and API concurrency.

```bash
# Quickstart (Docker)
git clone [https://github.com/tirupathijayadeep/bench-zero.git](https://github.com/tirupathijayadeep/bench-zero.git) && cd bench-zero
docker compose up --build -d
docker compose exec web pytest -v
```

---

#### 2. [Hostel Management System](https://github.com/tirupathijayadeep/hostel-management-system) — Role-Based Campus Operations Platform
> **Status:** Completed · **Role:** Full-Stack Backend Lead

* **Purpose:** Digitizes end-to-end hostel administration—replacing manual registers for room allocation, fee ledgers, leave approvals, visitor logs, and maintenance tickets.
* **Tech Stack:** `Python` · `Django` · `PostgreSQL` · `Bootstrap 5` · `Session Auth`
* **Key Engineering Contributions:**
  * Architected a custom user model enforcing a 3-tier **Role-Based Access Control (RBAC)** hierarchy (`Admin`, `Warden`, `Student`), scoping every view, queryset, and state transition to role permissions.
  * Implemented real-time in-app notifications, room condition audits, and hardened security defaults (CSRF/XSS mitigation, PBKDF2/Argon2 password hashing, strict session expiry).

```bash
# Quickstart (Local)
git clone [https://github.com/tirupathijayadeep/hostel-management-system.git](https://github.com/tirupathijayadeep/hostel-management-system.git) && cd hostel-management-system
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt && python manage.py migrate && python manage.py runserver
```

---

### Algorithmic Practice & Benchmarks

* **LeetCode (`200+` Solved):** Focused on optimal time/space complexity across **Sliding Window**, **Two-Pointer**, **Linked Lists**, **Greedy Algorithms**, and complex **SQL Window/Join Queries**.
* **Open to:** Backend Engineering Internships & SDE Roles (Python / Django / Distributed Systems).
