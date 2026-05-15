# AWS Automation Portfolio

## A collection of AWS reporting and billing automation projects

**Owner:** Hima Varsha M  
**Repository Name Suggestion:** `aws-automation-portfolio`  
**Default Branch:** `main`

---

## 1. Overview

This repository is planned as a portfolio of AWS automation projects. Each automation focuses on reducing manual reporting effort, improving consistency, and generating structured outputs for review or business use.

The repository can include multiple independent automation modules such as:

- Consolidated Report
- Invoice Automation
- RI Utilization Report

Each automation should have its own folder, script files, input folder, output folder, and README documentation.

---

## 2. Recommended Repository Structure

```text
aws-automation-portfolio/
|-- README.md
|-- .gitignore
|-- consolidated-report/
|   |-- README.md
|   |-- src/
|   |-- input/
|   |   `-- .gitkeep
|   `-- output/
|       `-- .gitkeep
|-- invoice-automation/
|   |-- README.md
|   |-- invoice-automation.py
|   |-- invoices/
|   |   `-- .gitkeep
|   `-- output/
|       `-- .gitkeep
`-- ri-utilization-report/
    |-- README.md
    |-- src/
    |-- input/
    |   `-- .gitkeep
    `-- output/
        `-- .gitkeep
```

---

## 3. Automation Modules

### 3.1 Consolidated Report

This folder can be used for automation that combines multiple reports or data sources into one final report.

Suggested folder name:

```text
consolidated-report
```

Suggested branch name:

```text
feature/consolidated-report
```

### 3.2 Invoice Automation

This folder contains the AWS invoice automation script. It reads invoice PDF files, extracts account-wise billing details, and generates Excel Invoice Reports.

Suggested folder name:

```text
invoice-automation
```

Suggested branch name:

```text
feature/invoice-automation
```

### 3.3 RI Utilization Report

This folder can be used for Reserved Instance utilization reporting automation.

Suggested folder name:

```text
ri-utilization-report
```

Suggested branch name:

```text
feature/ri-utilization-report
```

---

## 4. Branch Naming Standard

Use `main` as the default stable branch.

Recommended feature branches:

```text
feature/invoice-automation
feature/consolidated-report
feature/ri-utilization-report
```

Recommended documentation branches:

```text
docs/main-readme
docs/medium-article
```

Recommended bugfix branches:

```text
bugfix/invoice-total-formula
bugfix/pdf-parsing
bugfix/excel-formatting
```

---

## 5. GitHub Upload Guidelines

Upload only source code, documentation, and safe placeholder files.

Recommended files to commit:

```text
README.md
.gitignore
automation-folder/README.md
automation-folder/*.py
automation-folder/input/.gitkeep
automation-folder/output/.gitkeep
```

Do not commit confidential files such as:

```text
*.pdf
*.xlsx
*.csv
*.json
*.env
```

Real AWS billing reports, invoice PDFs, generated Excel files, and credential files should stay local.

---

## 6. Documentation Standard for Each Automation

Each automation folder should have its own `README.md` with:

- Purpose of the automation
- Access required
- Input files required
- Setup instructions
- Run command
- Output file details
- Common issues and fixes
- Owner details

This makes the repository easy to understand for freshers, reviewers, and future maintainers.

---

## 7. Ownership

This automation portfolio and its source code are owned by **Hima Varsha M**.

Each automation can be maintained, extended, and published by the owner.
