# Database Schema Specification

This section defines the complete relational database schema used by the Orchid Tracker.

---

## 🌱 Schema Philosophy

- Relational structure  
- Normalized care logs  
- Archival strategy  
- Schema evolution via auto‑healing  

---

## 🌿 Tables

### `orchids`
Primary specimen table.

### `watering_logs`
Watering events.

### `repotting_log`
Repotting events.

### `bloom_log`
Bloom periods.

### `observation_notes`
General observations.

### `archived_orchids`
Retired specimens.

---

## 🌸 Integrity Rules

- Foreign keys reference `orchids.id`  
- Logs are never deleted when a specimen is archived  
- Schema auto‑healing adds missing columns  

---

## 🌼 Related Sections

- [Architecture](architecture.md)  
- [Modules](modules.md)  
