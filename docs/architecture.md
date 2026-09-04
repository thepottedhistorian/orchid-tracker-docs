# Architecture Overview

This section defines the complete architectural structure of the Orchid Tracker application, including system layers, data flow, UI flow, module interactions, and schema auto‑healing logic.

---

## 🌱 Architectural Principles

- **Modularity** — Each subsystem is isolated  
- **Separation of concerns** — UI, database, ingestion, analytics  
- **Deterministic regeneration** — All modules can be rebuilt  
- **Schema auto‑healing** — Database evolves safely over time  

---

## 🌿 Directory Structure

```text
orchid_tracker/
│
├── main.py
├── config.py
├── database.py
│
├── utils/
│   └── id_parser.py
│
├── ui/
│   ├── widgets.py
│   ├── views/
│   │   ├── inventory_view.py
│   │   ├── accession_view.py
│   │   └── bulk_ops_view.py
│   │
│   ├── dialogs/
│   │   └── specimen_passport_dialog.py
│   │
│   └── modals/
│       ├── passport_modal.py
│       ├── system_modals.py
│       └── bulk_action_modals.py
│
└── assets/
    ├── orchid_icon.ico
    └── sample_photos/
```


---

## 🌸 Application Layers

- UI Layer  
- Database Layer  
- Relational Log Layer  
- Ingestion Engine Layer  
- Passport Modal Layer  
- Maintenance Layer  

---

## 🌼 Data Flow

1. User interacts with UI  
2. UI validates and formats data  
3. Database engine executes SQL  
4. UI renders updated views  
5. Logs stored in relational tables  
6. Passport analytics compute bloom/rest metrics  

---

## 🌿 Related Sections

- [Modules](modules.md)  
- [Database Schema](database-schema.md)  

