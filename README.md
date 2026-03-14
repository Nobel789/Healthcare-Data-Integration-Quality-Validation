# Healthcare-Data-Integration-Quality-Validation

Project Overview

Healthcare analysts often receive data from fragmented systems (Labs, Billing, Registration) in various formats. This project demonstrates the ability to import, clean, and validate multi-source healthcare data to ensure it is "analysis-ready."
Learning Objectives

    ETL Basics: Extracting, Transforming, and Loading data from disparate file formats.

    Format Handling: Managing .csv, .tsv, and .txt delimiters.

    Data Integrity: Performing "Pulse Checks" to verify Date of Birth (DOB) formatting and Patient ID consistency.

Technical Workflow

    Demographics Validation (.xlsx): Verified data types for 4 unique patients, ensuring DOB fields were recognized as Date objects for age calculations.

    Billing Data Import (.txt): * Imported claims data using a comma delimiter.

        Validated ProcedureCode as Text to prevent the loss of leading zeros (critical for medical billing accuracy).

    Lab Results Integration (.tsv): * Handled Tab-Separated Values from the Laboratory Information System (LIS).

        Verified column alignment for ResultValue and VisitID.

Data Quality Checklist

Before finalizing the datasets, I performed a "Pulse Check" to answer:

    Are all patient identifiers consistent across the Billing and Lab files?

    Are the Charge columns formatted as Currency/Numbers for financial reporting?

    Did the TSV import merge any text incorrectly?
