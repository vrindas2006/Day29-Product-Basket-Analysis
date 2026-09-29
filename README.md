# Day 29 - Product Basket Analysis

## 📌 Project Overview

This project focuses on Product Basket Analysis using the Online Retail II dataset.

The goal is to identify products that are frequently purchased together in the same transaction and use these relationships to generate simple product recommendations.

## 🎯 Objectives

- Analyze customer transaction data.
- Group products purchased within the same invoice.
- Identify frequently purchased product pairs.
- Determine the frequency of product combinations.
- Generate simple product recommendations.
- Understand customer purchasing patterns.

## 🛠️ Tools & Technologies

- Python
- Pandas
- Matplotlib
- Google Colab

## 📂 Dataset

The project uses the Online Retail II dataset.

The dataset contains transaction-level information such as:

- Invoice
- StockCode
- Description
- Quantity
- InvoiceDate
- Price
- Customer ID
- Country

## 🧹 Data Cleaning

The following cleaning steps were performed:

- Removed transactions with missing product descriptions.
- Removed cancelled invoices.
- Removed transactions with zero or negative quantities.
- Checked missing values after cleaning.

After cleaning, the dataset contained:

**512,033 rows and 8 columns.**

Customer ID had some missing values, but these rows were retained because Customer ID was not required for the product basket analysis.

## 🛒 Basket Creation

Products were grouped according to their Invoice ID.

Each invoice represents a customer transaction containing one or more products.

Example:

```text
Invoice
 ├── Product A
 ├── Product B
 └── Product C
