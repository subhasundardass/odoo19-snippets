# Odoo 19 Snippets

Professional code snippets for **Odoo 19** development. Boost your productivity with 50+ snippets covering Python models, XML views, security, actions, menus, cron jobs, and more — all updated for Odoo 19 conventions.

---

## ✨ Features

- ✅ Odoo 19 compatible (no deprecated `attrs`, `states` — uses new `invisible`, `readonly` syntax)
- ✅ Python snippets for models, fields, methods, wizards
- ✅ XML snippets for all view types (form, list, kanban, pivot, graph, calendar)
- ✅ Security snippets (groups, privileges, record rules)
- ✅ CSV snippets for `ir.model.access.csv`
- ✅ Tab stops for fast editing
- ✅ Covers all common patterns: compute, onchange, constrains, wizards, crons, email templates

---

## 🚀 Quick Start

Type the prefix and press `Tab` or `Enter` to expand.

---

## 📦 Python Snippets

### Model Definitions

| Prefix | Description |
|--------|-------------|
| `omodel` | Complete base model with mail thread |
| `oinherit` | Inherit and extend existing model |
| `owizard` | Transient wizard model |
| `osqlview` | SQL View model (non-stored report) |

### Fields

| Prefix | Description |
|--------|-------------|
| `om2o` | Many2one field |
| `oo2m` | One2many field |
| `om2m` | Many2many field |
| `oselection` | Selection field |
| `ocompute` | Computed field with `@api.depends` |
| `orelated` | Related field |
| `omonetary` | Monetary field with currency |

### Methods

| Prefix | Description |
|--------|-------------|
| `ocreate` | `create_multi` with auto sequence |
| `owrite` | Override write method |
| `ounlink` | Override unlink with state check |
| `ocopy` | Override copy/duplicate |
| `odefaultget` | Override `default_get` |
| `odisplayname` | Custom display name |
| `oonchange` | Onchange method |
| `oconstrains` | Field constraint validation |
| `oactionbtn` | State transition action button |
| `oreturnaction` | Return window action from button |
| `oemail` | Send email via template |
| `ocronmethod` | Scheduled action method with logging |
| `olog` | Logger setup and usage |
| `oerror` | Raise `UserError` |
| `ovalerror` | Raise `ValidationError` |

---

## 🗂️ XML Snippets

### Views

| Prefix | Description |
|--------|-------------|
| `oodoo` | XML file wrapper |
| `oform` | Complete form view |
| `olist` | List view with decorations |
| `okanban` | Kanban view |
| `osearch` | Search view with filters and group by |
| `opivot` | Pivot view |
| `ograph` | Graph view |
| `ocalendar` | Calendar view |
| `owizardform` | Wizard form view with footer buttons |

### Form Components

| Prefix | Description |
|--------|-------------|
| `obuttonbox` | Smart button box |
| `ostatbtn` | Stat button |
| `obtn` | Header button with invisible |
| `opage` | Notebook page |
| `oo2mlist` | Inline editable One2many list |
| `obadge` | Badge field with decorations |
| `omoney` | Monetary field in view |
| `ochatter` | Chatter component (Odoo 19 style) |
| `ofilter` | Search filter |
| `ogroupby` | Group by filter |

### Actions & Menus

| Prefix | Description |
|--------|-------------|
| `oaction` | Action window |
| `owizaction` | Wizard popup action |
| `oserveraction` | Server action (bulk action) |
| `ourlaction` | URL action |
| `omenuroot` | Root app menuitem |
| `omenu` | Child menuitem |

### Security

| Prefix | Description |
|--------|-------------|
| `oprivilege` | Privilege record (Odoo 17+) |
| `ogroup` | Security group with privilege |
| `orule` | Record rule (ir.rule) |

### Data

| Prefix | Description |
|--------|-------------|
| `osequence` | ir.sequence record |
| `ocron` | Cron scheduled action |
| `oemailtemplate` | Email template |
| `oreport` | QWeb PDF report action |

---

## 📋 CSV Snippets (`ir.model.access.csv`)

| Prefix | Description |
|--------|-------------|
| `ocsv` | CSV header row |
| `oaccessuser` | Access row for user group |
| `oaccessmanager` | Access row for manager group |
| `oaccessadmin` | Access row for admin group (full access) |
| `oaccessreadonly` | Access row read only |
| `oaccessfull` | Full block: user + admin rows |

---

## ⚙️ Recommended Settings

Add to your `.vscode/settings.json`:

```json
{
    "odoo.serverPath": "/usr/lib/python3/dist-packages/odoo",
    "files.associations": {
        "*.xml": "xml",
        "ir.model.access.csv": "csv"
    },
    "[xml]": {
        "editor.suggest.snippetsPreventQuickSuggestions": false
    },
    "[csv]": {
        "editor.suggest.snippetsPreventQuickSuggestions": false
    }
}
```

---

## 🔄 Odoo 19 Changes Covered

| Old (≤16) | New (17+/19) |
|-----------|--------------|
| `attrs="{'invisible': [...]}"` | `invisible="..."` |
| `attrs="{'readonly': [...]}"` | `readonly="..."` |
| `attrs="{'required': [...]}"` | `required="..."` |
| `<field name="comment">` on groups | Removed |
| `category_id` on groups | `privilege_id` |
| `<div class="oe_chatter">` | `<chatter>` wrapper |
| `tree` view type | `list` view type |

---

## 📝 License

MIT License — free to use, modify and distribute.

---

## 🤝 Contributing

Found a bug or want to add a snippet? Open an issue or PR on GitHub.

---

## 📌 Changelog

### 1.0.0
- Initial release
- 50+ snippets for Python, XML and CSV
- Full Odoo 19 compatibility
