# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## High-Level Code Architecture and Structure

*   **Purpose:** This repository contains a Python script (`ai_inventory_11_03_25.py`) for analyzing AI use case inventories from different years (2023, 2024, 2025).
*   **Data Sources:** The script reads raw AI inventory data from Excel files located in the `inventories/` directory. These files are typically sourced from external repositories (e.g., OMB's Federal AI Use Case Inventory).
*   **Data Processing:** The Python script uses the `pandas` library to load, clean, and process the inventory data. This includes handling missing values, stripping whitespace, identifying common use cases, and detecting duplicates.
*   **Analysis and Visualization:** The script performs various analyses, such as counting use cases, grouping data by department and agency, and comparing development stages. It uses `matplotlib` and `seaborn` to generate horizontal bar plots visualizing use case topic areas, impact designations (rights/safety-impacting, high-impact), and stages of development.
*   **Outputs:** The script generates new Excel files (`duplicate_use_cases_2023.xlsx`, `duplicate_use_cases_2024.xlsx`, `dev_stages_2023_2024.xlsx`, `groups_department_agency_2023_2024_2025.xlsx`) and PNG image files (plots) as output.

## Commonly Used Commands

*   **Run the analysis script:**
    ```bash
    python ai_inventory_11_03_25.py
    ```
