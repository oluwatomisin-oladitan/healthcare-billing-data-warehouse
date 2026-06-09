# Healthcare Clinic Billing Performance Data Warehouse

## Overview
A data warehouse built for a fictional healthcare clinic network to monitor 
and analyse billing performance across doctors, procedures, and time periods.
Built as part of a Business Intelligence course at Tilburg University.

## Architecture
Star schema with one fact table and five dimension tables.

| Table | Type | Description |
|-------|------|-------------|
| Fact_BillingPerformance | Fact | Billing amounts, appointment and billing counts |
| Dimension_Doctor | Dimension | Doctor specialization details |
| Dimension_Patient | Dimension | Patient information |
| Dimension_Procedure | Dimension | Medical procedure details |
| Dimension_BillingItem | Dimension | Billing item details |
| Dimension_Time | Dimension | Time context of billing |

## ETL Process
- Source data extracted from OLTP MySQL tables
- Transformed and loaded using KNIME Analytics Platform
- Dimension tables loaded first, followed by fact table

## My Contributions
- Built KNIME Workflow 2: all dimension tables (Doctor, Patient, Procedure, BillingItem)
- Built KNIME Workflow 3: Fact_BillingPerformance table
- Created BillingPerformanceSummary SQL view

## Files
- Healthcare_Clinic_OLTP_final.mwb — OLTP schema
- Healthcare_Clinic_DW.mwb — Data warehouse schema
- Report_BillingPerformance_final.knwf — KNIME ETL workflow
- View_BillingPerformanceSummary_final.sql — SQL billing summary view

## Technologies
- MySQL
- KNIME Analytics Platform
- Star Schema / Data Warehousing
- SQL
