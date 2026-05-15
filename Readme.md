# AWS Automation Portfolio

## A collection of AWS reporting and billing automation projects

**Owner:** Hima Varsha M  
**Repository:** `aws-automation-portfolio`  
**Branch:** `cost-automation-codes`

---

## 1. Overview

This branch contains AWS automation projects focused on reducing manual reporting effort, improving consistency, and generating structured outputs for review or business use.

The following automation modules are available in this branch:

- Consolidated Report
- Invoice Automation
- RI Utilization Report

Each automation has its own folder, script files, input folder, output folder, and README documentation.

---

## 2. Branch Structure

> You are currently on the `cost-automation-codes` branch. All folders and scripts below are available in this branch.

```text
cost-automation-codes/
|-- README.md
|-- main.gitignore
|-- Consolidated Report/
|   |-- README.md
|   |-- consolidated-automation.py
|   |-- accounts.txt
|   |-- Month1/
|   |   `-- 123456789012_account_report.csv
|   `-- Month2/
|       `-- 123456789012_account_report.csv
|-- Invoice Automation/
|   |-- README.md
|   |-- invoice-automation.py
|   |-- generate_dummy_invoices.py
|   |-- read_invoices.py
|   |-- .gitignore
|   |-- assets/
|   |   `-- screenshots/
|   |       `-- .gitkeep
|   `-- invoices/
|       `-- .gitkeep
`-- RI Utilization Report/
    |-- README.md
    |-- utilization-automation.py
    `-- Month - YYYY/
        `-- reservations-utilization-table - *.csv
```

---

## 3. Automation Modules

### 3.1 Consolidated Report

Combines multiple AWS billing CSV reports across accounts and months into a single consolidated Excel report.

| Field  | Details                                              |
|--------|------------------------------------------------------|
| Folder | `Consolidated Report/`                               |
| Script | `consolidated-automation.py`                         |
| Input  | Monthly CSV files per account (`Month1/`, `Month2/`) |
| Config | `accounts.txt`                                       |
| Output | Consolidated Excel report                            |

### 3.2 Invoice Automation

Reads AWS invoice PDF files, extracts account-wise billing details, and generates a structured Excel Invoice Report.

| Field  | Details                                                                                                                      |
|--------|------------------------------------------------------------------------------------------------------------------------------|
| Folder | `Invoice Automation/`                                                                                                        |
| Script | `invoice-automation.py`                                                                                                      |
| Input  | Invoice PDFs placed in `invoices/`                                                                                           |
| Output | Excel Invoice Report                                                                                                         |
| Extras | `generate_dummy_invoices.py` for testing, `read_invoices.py` for extraction, `assets/screenshots/` for documentation visuals |

### 3.3 RI Utilization Report

Processes Reserved Instance utilization CSV exports from AWS Cost Explorer and generates a summarized Excel report.

| Field  | Details                                                   |
|--------|-----------------------------------------------------------|
| Folder | `RI Utilization Report/`                                  |
| Script | `utilization-automation.py`                               |
| Input  | RI utilization CSVs per account/service (`Month - YYYY/`) |
| Output | RI Utilization Excel report                               |

---

## 4. GitHub Upload Guidelines

Upload only source code, documentation, and safe placeholder files.

**Commit these files:**

```text
README.md
main.gitignore
automation-folder/README.md
automation-folder/*.py
automation-folder/input/.gitkeep
automation-folder/output/.gitkeep
```

**Do not commit confidential files:**

```text
*.pdf
*.xlsx
*.csv
*.json
*.env
```

Real AWS billing reports, invoice PDFs, generated Excel files, and credential files should stay local.

---

## 5. Documentation Standard for Each Automation

Each automation folder has its own `README.md` with:

- Purpose of the automation
- Access required
- Input files required
- Setup instructions
- Run command
- Output file details
- Common issues and fixes
- Owner details

---

## 6. Ownership

This branch and its source code are owned by **Hima Varsha M**.
