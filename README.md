# Inventory Management System (Excel)

An Excel-based Inventory Management System that tracks the full cycle of 
a small business's stock — from purchase to sale to remaining inventory — 
with automated calculations and low-stock alerts.

## Overview

Unlike a static reporting dashboard, this project focuses on connecting 
different parts of a business process: Customers, Products, and Vendors 
are linked to live Purchase and Sales entries, and stock levels update 
automatically as new transactions are added.

## Features

- **Multi-sheet relational structure** — Customers, Products, and Vendors 
  master data linked to Purchase and Sales tables via VLOOKUP
- **Dropdown-based data entry** — Data Validation dropdowns for HSN Code 
  and Customer ID prevent typing errors during entry
- **Automatic stock calculation** — Stock = Purchased Units − Sold Units, 
  recalculated live using SUMIF across linked tables
- **Automated low-stock alerts** — When stock falls below a threshold, 
  the dashboard flags the product along with the vendor's contact number, 
  pulled automatically from the Vendors sheet
- **Summary dashboard** — KPI cards (Purchase Amount, Sales Amount, Stock 
  Value, Profit/Loss) plus Top 5 Customers and Top 5 Products charts, 
  built on PivotTables

## Tools & Techniques Used

- Excel Tables with structured references
- VLOOKUP, SUMIF, IFERROR
- Data Validation (dropdown lists)
- PivotTables and GETPIVOTDATA
- INDEX + AGGREGATE (to compile only active alerts into a clean list, 
  skipping blanks)

## Screenshots

[Dashboard]<img width="1920" height="1080" alt="dashboard-screenshot" src="https://github.com/user-attachments/assets/f3013106-0343-48f2-bd4e-edb9ab8d17dc" />

[Sales Entry]<img width="1920" height="1080" alt="sales-screenshot" src="https://github.com/user-attachments/assets/afa5fa0a-30f2-43cc-a343-1dc874bd6092" />

[Inventory Tracking]<img width="1920" height="1080" alt="inventory-screenshot" src="https://github.com/user-attachments/assets/90dae96d-671d-436b-aca0-f4a3f3f7a3c8" />

## Video

[Dashboard]<mp4 https://github.com/user-attachments/assets/aa910f5a-c1c1-40b5-a7ac-017a957facc9

## What I'd Improve Next

- Rebuild the stock calculation using fully table-referenced SUMIF formulas 
  for better robustness as data grows
- Add Power Query for cleaner data import/cleanup
- Move some calculations to Power Pivot / DAX for scalability

## Note

This project uses a self-created sample dataset for practice purposes, 
not real business data.
