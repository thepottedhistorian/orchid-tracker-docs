---
title: Module‑by‑Module Breakdown
nav_order: 3
---

# Module‑by‑Module Breakdown

This section provides a detailed breakdown of every module in the Orchid Tracker application.

---

## 🌿 Core Modules

### `main.py`
Application entrypoint and controller.

### `config.py`
Global configuration, theme palette, metadata, and paths.

### `database.py`
SQLite engine, schema creation, and auto‑healing.

### `utils/id_parser.py`
Parses ID ranges like `1-5, 7, 10-12`.

### `ui/widgets.py`
Shared UI components (TopmostModal, StatusDot).

---

## 🌱 UI Views

### `inventory_view.py`
Primary ledger interface.

### `accession_view.py`
Accession form and spreadsheet ingestion engine.

### `bulk_ops_view.py`
Bulk watering and repotting interface.

---

## 🌸 Dialogs & Modals

### `specimen_passport_dialog.py`
Compact Passport File dialog.

### `passport_modal.py`
Full‑screen Passport File with analytics and photo carousel.

### `system_modals.py`
Help, care guides, changelog, about modal, archive catalog.

### `bulk_action_modals.py`
Bulk watering and repotting dialogs.

---

## 🌼 Related Sections

- [Architecture](architecture.md)  
- [Regeneration Prompts](regeneration.md)  
