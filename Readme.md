# CyberShield Training Automation Dashboard

Enterprise-grade browser-based dashboard for automating cybersecurity training compliance workflows and generating structured Excel reports.

Source File: 

---

# Capabilities

* Multi-module training processing
* Drag & drop Excel ingestion
* Dynamic Excel header detection
* Employee correlation via:

  * Employee ID
  * Work Email
* Automated transcript status resolution
* Duplicate elimination
* Year-wise report segregation
* Pending-user extraction
* Multi-sheet Excel export
* Real-time KPI dashboard

---

# Supported Training Modules

| Module                      | Base File | Tool Output |
| --------------------------- | --------- | ----------- |
| Application Security        | ❌         | ✅           |
| Growth Group                | ❌         | ✅           |
| New Joiner                  | ❌         | ✅           |
| BSC                         | ✅         | ✅           |
| Phishing Normal             | ✅         | ✅           |
| Band 4+ / Senior Management | ✅         | ✅           |

---

# Core Processing Engine

The dashboard performs:

1. Excel parsing via SheetJS
2. Dynamic schema discovery
3. User matching & normalization
4. Transcript status calculation
5. Year-based segmentation
6. Excel report generation

---

# Output Structure

Generated reports contain:

* Employee ID
* Work Email Address
* Macro Entity Level 2 (Zone)
* Transcript Status
* Training Start Date
* Transcript Completed Date

---

# Processing Rules

| Condition                     | Result                     |
| ----------------------------- | -------------------------- |
| Completed date exists         | Completed                  |
| Status contains "In Progress" | In Progress                |
| Empty status                  | Not Started                |
| Otherwise                     | Original transcript status |

---

# Architecture

* Pure client-side application
* No backend dependency
* No database dependency
* No external storage
* Local browser-based processing

---

# Workflow

## 1. Open Dashboard

```
Dashboard.html
```

## 2. Select Module

* App Security
* Growth
* New Joiner
* BSC
* Phishing Normal
* Band 4+

## 3. Upload Files

Depending on module:

* Base Userbase Excel
* Tool Output Excel

## 4. Set Assignment Date

Select assignment date from the UI.

## 5. Run Processing

Click:

```
Calculate
```

## 6. Export Reports

Available exports:

* Full Output Workbook
* Pending Users Workbook

---

# Key Features

* Modern enterprise UI
* Real-time KPI metrics
* Year-wise tab segregation
* Automated progress tracking
* Dynamic upload validation
* Toast notification system
* Responsive layout
* High-volume Excel handling

---

# Browser Support

Recommended:

* Google Chrome
* Microsoft Edge

---

# Security Model

* Fully offline-compatible
* No server-side processing
* No outbound data transfer
* Local file-only operations

---

# Main File

```
Dashboard.html
```
