---
title: "AI-Powered Financial Data Analysis Tool with MCP"
excerpt: "An AI-driven Excel financial data analysis tool built with Python, Pandas, and Model Context Protocol (MCP), connecting natural language instructions with deterministic data processing."
collection: portfolio
---


## Project Overview

This project explored how AI and programming can be applied to repetitive financial data-processing tasks.

Using **Python, Pandas, and Model Context Protocol (MCP)**, I built an AI-driven financial data analysis tool that connects natural language instructions with structured Excel data processing.

The system follows an:

**AI → MCP → Python → Excel**

workflow, allowing users to interact with financial datasets through natural language while keeping data processing and numerical calculations deterministic and reproducible.

## MCP Architecture

A local **MCP Server** was developed using the Python MCP SDK.

Data-analysis functions were packaged as independent tools that can be called by an AI model according to the user's request.

The workflow can be summarized as:

**User's Natural Language Request**  
↓  
**AI Understanding & Tool Selection**  
↓  
**MCP Tool Call**  
↓  
**Python / Pandas Processing**  
↓  
**Excel Data**  
↓  
**Calculated Result**  
↓  
**AI Natural Language Explanation**

This architecture separates natural language understanding from deterministic data processing.

## Read Module

The **Read** module was developed using Pandas to provide structured Excel data inspection.

The module supports:

- Reading Excel files
- Identifying multiple worksheets
- Reporting row and column dimensions
- Identifying field names and data types
- Previewing data
- Checking missing values and missing-value rates
- Detecting duplicate records
- Identifying unique values
- Calculating descriptive statistics for numerical fields, including mean, median, maximum, and minimum

These functions provide an initial data-quality assessment before further financial analysis.

## Finance Module

The **Finance** module encapsulates common financial analysis logic into callable tools.

The module is designed to allow AI to invoke predefined financial calculation functions based on the user's analytical requirements.

It supports financial analysis at both the **company and industry levels**, reducing the need to manually write repetitive Excel formulas and perform repeated calculations.

## Data Processing Module

The **Data Processing** module uses Pandas to perform structured data manipulation.

The module includes functions for:

- Data filtering
- Grouping and aggregation
- Field processing
- Data organization
- Preparing datasets for subsequent financial analysis

This creates a standardized data-processing layer between raw Excel data and downstream financial analysis.

## Large-Scale Excel Data Testing

The tool was tested using approximately **17,500 rows × 27 columns** of listed-company financial data covering multiple years from **2019 to 2024**.

The test dataset was used to evaluate:

- Excel data reading
- Data-quality inspection
- Missing-value analysis
- Duplicate detection
- Financial data processing
- Tool invocation and result generation

This provided a practical test case for evaluating the tool's ability to handle relatively large structured financial datasets.

## AI-Assisted Data Analysis

The project adopted a hybrid approach combining AI with deterministic computation.

The AI layer is responsible for:

- Understanding natural language requests
- Identifying the appropriate analytical operation
- Selecting the corresponding MCP tool
- Explaining the resulting analysis in natural language

Python and Pandas are responsible for:

- Reading the actual data
- Performing calculations
- Processing datasets
- Generating numerical results

This approach reduces the risk of an AI model estimating or generating unsupported numerical results directly.

## Reproducible Analytical Workflow

The key design principle was to separate **reasoning from computation**.

Instead of asking an AI model to directly calculate financial results from an Excel file, the model calls predefined Python tools through MCP.

This creates a more controlled workflow in which:

**AI handles interpretation → MCP handles tool communication → Python handles computation → AI explains the results**

The resulting architecture provides a foundation for extending the tool with additional financial analysis and data-processing functions.

## Core Modules

The current implementation includes three main modules:

| Module | Main Function |
| --- | --- |
| **Read** | Excel reading and data-quality inspection |
| **Finance** | Financial indicator calculation and analysis |
| **Data Processing** | Filtering, grouping, aggregation, and data transformation |

## Tools

**Python · Pandas · MCP · Excel · AI-assisted Programming · GitHub**

## Key Takeaway

This project combines my accounting and financial background with practical programming and AI skills.

It demonstrates how financial data-processing workflows can be transformed from repetitive manual Excel operations into reusable, AI-accessible analytical tools.

The project also provided hands-on experience with **MCP architecture, Python/Pandas data processing, financial analysis, and AI-assisted programming**, while maintaining deterministic and reproducible numerical calculations.
