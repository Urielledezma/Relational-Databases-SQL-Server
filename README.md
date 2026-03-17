# Relational Databases in SQL Server — Practical Design, Normalization & Querying

[![SQL Server](https://img.shields.io/badge/SQL%20Server-2019%2B-red)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.txt)
[![Status](https://img.shields.io/badge/status-active-brightgreen)](#)

A practical **relational databases** repository in **SQL Server** built to be both:
- an **academic and portfolio-facing repo** (clean structure, reproducible scripts, project-based organization), and
- a **public reference** for anyone learning or revisiting core relational database concepts.

This repo collects coursework, exercises, and projects developed throughout a semester of **Relational Databases**, with a focus on:
- **relational modeling**
- **normalization**
- **schema design**
- **queries**
- **views**
- **stored procedures**
- **constraints and sample data workflows**

---

## Learning map (recommended path)

| Module | What you’ll learn | Where to look |
|---|---|---|
| 00 — Setup & foundations | How the repo is organized, how to run scripts, SQL Server workflow basics | `README.md` + `notes/` |
| 01 — Relational modeling | Entities, attributes, keys, relationships, schema planning | `notes/` + `projects/*/README.md` |
| 02 — Normalization | 1NF, 2NF, 3NF, dependency thinking, redundancy reduction | `projects/whatsapp-normalization/` + `notes/` |
| 03 — Schema creation | Tables, PK/FK constraints, data types, integrity rules | `projects/*/schema/` |
| 04 — Sample data & DML | Inserts, updates, deletes, realistic test data | `projects/*/seed/` |
| 05 — Querying | Filtering, joins, grouping, subqueries, practical SQL querying | `projects/*/queries/` |
| 06 — Views & procedural SQL | Views, stored procedures, reusable SQL logic | `projects/*/views/` + `projects/*/procedures/` |
| 07 — Integrated projects | End-to-end mini database projects with scripts and documentation | `projects/` |

> Tip: Start with a project README first, then explore its `schema/`, `seed/`, `queries/`, and `procedures/` folders in order.

---

## What you’ll find here

### Core topics (practical)
- Relational schema design
- Primary keys and foreign keys
- Constraints and integrity rules
- Database normalization
- DDL and DML workflows
- Practical SQL querying with joins, grouping, and subqueries
- Views for reusable query logic
- Stored procedures for procedural SQL tasks
- Reproducible project scripts organized by purpose

### What this repo is not
- Not a theory-only collection
- Not a production application backend
- Not a dump of raw database files
- Not tied to one single project or domain

---

## Who this is for
- **Students** learning relational database design in a hands-on way
- **Beginners in SQL Server** who want runnable, structured examples
- **Recruiters / hiring managers** reviewing academic SQL work in portfolio format
- **Anyone** who needs a practical reference for schema design, normalization, and SQL querying

---

## Repository structure

```text
.
├── projects/
│   ├── project-database/
│   │   ├── schema/         # CREATE DATABASE / CREATE TABLE / constraints
│   │   ├── seed/           # INSERT statements and sample data
│   │   ├── queries/        # SELECT queries, joins, reports, exercises
│   │   ├── views/          # CREATE VIEW scripts
│   │   ├── procedures/     # Stored procedures
│   │   └── README.md       # Project-specific context and usage
│   ├── whatsapp-normalization/
│   ├── games/
│   ├── instrument-store/
│   └── procedures-practice/
├── notes/                  # Concept notes (normalization, keys, modeling, etc.)
├── docs/
│   ├── diagrams/           # ER diagrams, relational diagrams, screenshots
│   └── screenshots/        # Optional visual references
├── .gitignore
├── LICENSE.txt
└── README.md
```

---

## Quickstart (copy/paste friendly)

### 1) Requirements

* **SQL Server**
* **SQL Server Management Studio (SSMS)**

Optional:

* **Azure Data Studio** for lightweight script editing
* **Git** for version control and cloning

### 2) Clone

```bash
git clone https://github.com/Urielledezma/Relational-Databases-SQL-Server.git
cd Relational-Databases-SQL-Server
```

### 3) Open a project

Choose any folder inside `projects/`, then run the scripts in a logical order:

1. `schema/`
2. `seed/`
3. `queries/`
4. `views/`
5. `procedures/`

### 4) Run in SQL Server

Open the `.sql` files in **SSMS** and execute them against your local SQL Server instance.

A typical workflow is:

* create the database
* create tables and constraints
* insert sample data
* test queries
* create views and procedures

---

## Repository philosophy

Relational database work is more than writing isolated queries.

This repo emphasizes:

* clear database structure
* good naming and organization
* separation of schema, data, and logic
* reproducible SQL workflows
* portfolio-ready presentation of academic projects

The goal is to make each project easy to:

* read
* run
* explain
* extend

---

## Project organization philosophy

Each database project is organized by responsibility:

* `schema/` for structure
* `seed/` for sample data
* `queries/` for exploration and reporting
* `views/` for reusable query abstractions
* `procedures/` for procedural database logic

This keeps projects modular and easier to maintain than storing everything in one large SQL file.

---

## Data policy

This repository is intended to store **SQL scripts**, not raw SQL Server engine files.

Do **not** commit:

* `.mdf`
* `.ldf`
* `.ndf`
* `.bak`
* temporary or machine-specific database files

Preferred approach:

* store **schema scripts**
* store **sample/seed data scripts**
* store **query, view, and procedure scripts**
* document how to recreate each database from scratch

---

## Code conventions

* Use `snake_case` or consistent SQL naming conventions across each project
* Prefer meaningful table and column names
* Separate files by responsibility whenever possible
* Keep scripts idempotent when practical
* Add comments when business rules or logic are not obvious

Suggested folder/file patterns:

* `schema/01_create_database.sql`
* `schema/02_create_tables.sql`
* `schema/03_constraints.sql`
* `seed/01_insert_sample_data.sql`
* `queries/01_basic_selects.sql`
* `queries/02_joins_and_aggregations.sql`
* `views/01_create_views.sql`
* `procedures/01_stored_procedures.sql`

---

## Current and planned contents

This repo may include projects and exercises such as:

* relational modeling practice
* normalization exercises
* academic mini-project databases
* query collections
* stored procedure exercises
* documentation and diagrams for database design

As the repo evolves, projects may be reorganized and documented more thoroughly for clarity and reproducibility.

---

## Roadmap

* [ ] Export and organize all course databases as reusable `.sql` scripts
* [ ] Add full folder structure for each project
* [ ] Add project-level README files
* [ ] Add normalization notes and examples
* [ ] Add ER diagrams / relational diagrams
* [ ] Add views and stored procedure examples where available
* [ ] Improve naming consistency across scripts
* [ ] Add screenshots or schema visuals in `docs/`
* [ ] Polish documentation for portfolio presentation

---

## Contributing

Contributions are welcome, especially:

* typo fixes
* clearer explanations
* better SQL script organization
* improvements to documentation
* additional academic examples with clear structure

Please open an Issue or Pull Request describing:

* what you changed
* why it improves the repo
* how it should be used or reviewed

---

## License

MIT — see [`LICENSE.txt`](LICENSE.txt).

---

## Citation

```bibtex
@misc{relational_databases_sql_server_urielledezma,
  author       = {Urielledezma},
  title        = {Relational Databases in SQL Server: Practical Design, Normalization and Querying},
  year         = {2026},
  publisher    = {GitHub},
  howpublished = {\url{https://github.com/Urielledezma/Relational-Databases-SQL-Server}},
  note         = {MIT License}
}
```
