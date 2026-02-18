# Automation Portfolio

A curated portfolio of small, practical automation projects demonstrating Python workflows for data collection and file operations. Current projects include:

*   **Automated Crypto Web Scraper (V2)** – pulls market data on a schedule and structures it for quick analysis. [\[github.com\]](https://github.com/jmillerw101/Automation-Portfolio)
*   **Automatic File Sorter** – watches a directory and organizes files into folders by type and rules. [\[github.com\]](https://github.com/jmillerw101/Automation-Portfolio)

***

## Why this portfolio?

As a Quality Technician moving toward advanced Quality/Automation, I build small, focused tools that remove repetitive work, capture clean data, and make results easy to audit. These projects reflect the same principles I apply at work—clear inputs/outputs, traceability, and maintainable code.

***

## Projects

### 1) Automated Crypto Web Scraper (V2)

**Goal:** Programmatically collect cryptocurrency market data for time‑series tracking or quick analysis.

**Highlights**

*   Consistent schema for downstream use (Excel, pandas, Power BI).
*   Simple scheduling via OS task scheduler or `cron`.
*   Clear separation of config (tickers, intervals) from logic.

**What’s inside**

*   Notebook: `Automated Crypto Web Scraper V2.ipynb` [\[github.com\]](https://github.com/jmillerw101/Automation-Portfolio)
*   Typical stack: `requests`/`httpx`, `pandas`, `time`/`schedule`.

**Try it quickly**

1.  Create and activate a virtual environment.
2.  Install requirements (example):
    ```bash
    pip install pandas requests python-dotenv
    ```
3.  Open the notebook and run all cells.
4.  (Optional) Export outputs to CSV for dashboards.

***

### 2) Automatic File Sorter

**Goal:** Keep a “Downloads” or “Intake” folder clean by automatically routing files into rule‑based subfolders.

**Highlights**

*   Rule table for extensions → destination folder.
*   Optional timestamping to prevent collisions.
*   Dry‑run mode to preview actions.

**What’s inside**

*   Notebook: `Automatic File Sorter.ipynb` [\[github.com\]](https://github.com/jmillerw101/Automation-Portfolio)
*   Typical stack: `pathlib`, `shutil`, `os`, `re`.

**Try it quickly**

1.  Define a source folder (e.g., `~/Downloads`) and mapping:
    ```python
    RULES = {
        ".pdf": "Documents/PDFs",
        ".xlsx": "Documents/Excel",
        ".csv": "Data/CSV",
        ".jpg": "Media/Images"
    }
    ```
2.  Run the notebook cells to preview → then execute the move.
3.  (Optional) Schedule hourly with Task Scheduler or `cron`.

***


## Project Structure

    Automation-Portfolio/
    ├─ Automated Crypto Web Scraper V2.ipynb
    ├─ Automatic File Sorter.ipynb
    └─ README.md

(See repository file list on GitHub.) [\[github.com\]](https://github.com/jmillerw101/Automation-Portfolio)

***

## How I design these automations

*   **Reliability first:** deterministic inputs/outputs, idempotent where possible.
*   **Traceability:** explicit logs and CSV outputs to support audits.
*   **Maintainability:** isolate config from code; small, single‑purpose functions.
*   **Scalability:** start as notebooks → promote to scripts/CLI if usage grows.

***

## Results & Impact (examples)

*   **Time saved:** File sorting replaces manual housekeeping; scraping removes copy/paste from web sources.
*   **Data quality:** Standardized schemas make trend analysis reliable.
*   **Auditability:** CSV logs and consistent naming support review and compliance needs.

***

## About Me

I’m **Justin Miller**, a Quality Technician focused on building practical automation that improves accuracy and frees teams from repetitive work. I’m growing toward Quality Specialist/Automation roles and open to collaboration or consulting engagements.

*   **Primary tools:** Python, pandas, Jupyter, Excel
*   **Domains:** Quality systems, data cleanup, reporting automation
*   **Contact:** `jmillerw101@gmail.com`

***

## Contributing

Have an idea, bug, or enhancement? Open an issue or PR with a clear description, steps to reproduce (if applicable), and proposed changes. For new utilities, include a small example dataset or screenshots.

***

## Notes for reviewers

*   This repository currently contains two Jupyter notebooks and a README; no external datasets are included. [\[github.com\]](https://github.com/jmillerw101/Automation-Portfolio)

***

