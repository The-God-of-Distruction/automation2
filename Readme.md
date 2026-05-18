# CyberShield Training Automation Dashboard

Modern browser-based automation dashboard for processing cybersecurity training compliance data and generating year-wise Excel reports.

---

# Features

* Multi-section training processing
* Excel upload + parsing
* Dynamic header detection
* Employee ID / Email matching
* Auto status calculation
* Duplicate handling
* Year-wise output split (2024 / 2025 / 2026)
* Pending user extraction
* Excel export generation
* Fully client-side processing

---

# Supported Modules

| Module          | Base File | Tool Output |
| --------------- | --------- | ----------- |
| App Security    | ❌         | ✅           |
| Growth Group    | ❌         | ✅           |
| New Joiner      | ❌         | ✅           |
| BSC             | ✅         | ✅           |
| Phishing Normal | ✅         | ✅           |
| Band 4+         | ✅         | ✅           |

---

# Core Processing Logic

The dashboard:

1. Reads uploaded Excel files
2. Detects headers dynamically
3. Matches users via:
   * Employee ID
   * Email Address
4. Determines training status
5. Splits output by year
6. Generates downloadable reports

---

# Output Columns

* Employee ID
* Work Email Address
* Macro Entity Level 2 (Zone)
* Transcript Status
* Training Start Date
* Transcript Completed Date

---

# Status Rules

| Condition              | Status          |
| ---------------------- | --------------- |
| Completed date exists  | Completed       |
| "In Progress" detected | In Progress     |
| Empty status           | Not Started     |
| Otherwise              | Original Status |

---

# Usage

## 1. Open Dashboard

```text
Dashboard.html
```

---

## 2. Upload Files

Depending on module:

* Base Userbase Excel
* Tool Output Excel

---

## 3. Set Assignment Date

Select the assignment date from the date picker.

---

## 4. Process

Click:

```
Calculate
```

---

## 5. Export

Available downloads:

* Full Output Excel
* Pending Users Excel

---

# Architecture

* Fully client-side
* No backend
* No database
* No external storage
* Local browser processing only

---

# Browser Support

Recommended:

* Google Chrome
* Microsoft Edge

---

# Notes

* Supports drag & drop uploads
* Handles duplicate users automatically
* Optimized for ABI training workflows
* Year-based report segregation included

---

# Main File

```text
Dashboard.html
```
