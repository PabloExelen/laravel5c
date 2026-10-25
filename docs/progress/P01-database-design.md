# P01: Database Design and Table Relationships

| | |
|---|---|
| **Status** | 🚧 In progress |
| **Started** | 2026-10-25 |
| **Completed** | - |
| **Branch** | `feature/p01-database-design` |
| **Pull request** | [PRs by USERNAME-YUSUF](https://github.com/mirzayogy/laravel5d/pulls?q=is%3Apr+author%3AUSERNAME-YUSUF) |

## Goal
Design and implement the database of the **CafeOrder** cafe menu ordering system, focusing on table relationships with Eloquent: One-to-One, One-to-Many, Many-to-Many (with pivot data), and Has-Many-Through.

## Jobs

| Code | Job | Status | Completed | Proof |
|---|---|---|---|---|
| J1 | Database design, ERD, and README | ✅ Done | 2026-10-25 | [erd.md](../database/erd.md), [README.md](../../README.md) |
| J2 | Progress report | ✅ Done | 2026-10-25 | [branch commits](https://github.com/USERNAME-YUSUF/laravel5d/commits/feature/p01-database-design) |
| J3 | Migrations | ⏳ Planned | - | - |
| J4 | Models and relationships | ⏳ Planned | - | - |
| J5 | Factories and seeders | ⏳ Planned | - | - |

**Status legend:** ⏳ Planned · 🚧 In progress · ✅ Done · ⛔ Blocked

---

### J1: Database design, ERD, and README
- **Status:** ✅ Done, 2026-10-25
- **What:** 8 tables covering every relationship type. `order_items` is the pivot between orders and menus and carries `quantity` and `unit_price`. The root README describes the project and contains the same Mermaid diagram as `erd.md`.
- **Proof:** [`docs/database/erd.md`](../database/erd.md), [`README.md`](../../README.md), [branch commits](https://github.com/USERNAME-YUSUF/laravel5d/commits/feature/p01-database-design)
- **Verified:** the Mermaid diagram renders on the GitHub pages of `README.md` and `erd.md`.
- **Not done:** migrations and models for these tables.

### J2: Progress report
- **Status:** ✅ Done, 2026-10-25
- **What:** This file, recording phase P01 with its jobs, status, and proof.
- **Proof:** [`docs/progress/P01-database-design.md`](P01-database-design.md), [branch commits](https://github.com/USERNAME-YUSUF/laravel5d/commits/feature/p01-database-design)

### J3: Migrations
- **Status:** ⏳ Planned
- **What:** Table migrations for the 8 tables, with foreign keys, cascade and restrict rules, and unique constraints as described in the ERD design notes.

### J4: Models and relationships
- **Status:** ⏳ Planned
- **What:** Eloquent models with `hasOne`, `hasMany`, `belongsTo`, `belongsToMany` (with `withPivot`), and `hasManyThrough`.

### J5: Factories and seeders
- **Status:** ⏳ Planned
- **What:** Factories for all models, a category seeder (6 categories), and a database seeder with sample menus, tags, users, and orders.

---

## Next
Finish J3 to J5, then update this file and the PR description. Later phases get their own file in this folder, for example `P02-authentication-and-menu.md`, each with its own jobs (J1, J2, ...).

Reference jobs in commit messages, for example `P01-J3: add menus migration`.