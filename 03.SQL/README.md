# 🗄️ SQL: Structured Query Language

<div align="center">

![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)
![Level](https://img.shields.io/badge/Level-Beginner%20to%20Advanced-blue?style=flat-square)
![Language](https://img.shields.io/badge/Language-SQL%2FTSQL-blue?style=flat-square)
![Topics](https://img.shields.io/badge/Topics-8-purple?style=flat-square)

**Master SQL: From Basics to Advanced Database Operations**

[Overview](#overview) • [Learning Objectives](#-learning-objectives) • [Topics](#-core-sql-topics) • [Key Functions](#-key-sql-functions)

</div>

---

## Overview

**SQL** (Structured Query Language) is the standard, universal language for managing and querying relational databases. This comprehensive module covers essential SQL concepts, from fundamental queries to advanced database operations, enabling you to efficiently retrieve, manipulate, and analyze data from databases.

### Why SQL?
- 🌍 Universal standard for all relational databases
- 💼 Essential skill for data professionals
- 🚀 High performance for large datasets
- 📊 Foundation for business intelligence and analytics
- 🔐 Secure data access and management

---

## 📚 Learning Objectives

After completing this module, you will be able to:

- ✅ Understand relational database concepts and design
- ✅ Write efficient and optimized SQL queries
- ✅ Master data manipulation (CRUD operations)
- ✅ Retrieve and analyze data using joins and aggregations
- ✅ Apply advanced querying techniques
- ✅ Design normalized database schemas
- ✅ Ensure data integrity and consistency
- ✅ Optimize query performance

---

## 📂 Core SQL Topics

### **1. Database Fundamentals** 🏛️
Understanding relational databases
- **Relational Database Concepts**
  - ACID properties and transactions
  - Constraints and data integrity
  - Schema design principles
  
- **Tables, Rows, and Columns**
  - Data types and constraints
  - Primary keys and unique constraints
  - Foreign keys and relationships
  
- **Data Normalization**
  - First Normal Form (1NF)
  - Second Normal Form (2NF)
  - Third Normal Form (3NF)
  - Avoiding data redundancy

### **2. Basic Queries** 🔍
Fundamental SQL operations
- **SELECT Statements**
  - Selecting specific columns
  - Selecting all columns with *
  - Column aliases and expressions
  
- **WHERE Clauses and Filtering**
  - Comparison operators (=, <>, <, >, <=, >=)
  - Logical operators (AND, OR, NOT)
  - IN and BETWEEN operators
  - LIKE for pattern matching
  - IS NULL for null values
  
- **ORDER BY and Sorting**
  - Ascending and descending order
  - Sorting by multiple columns
  
- **DISTINCT and Unique Values**
  - Removing duplicates
  - Count of distinct records

### **3. Data Manipulation** 📝
Creating, updating, and deleting data
- **INSERT:** Adding new records to tables
  - Single row insertion
  - Multiple row insertion
  - INSERT from SELECT queries
  
- **UPDATE:** Modifying existing data
  - Conditional updates with WHERE
  - Updating multiple columns
  - Safety considerations
  
- **DELETE:** Removing records
  - Conditional deletion
  - Truncate vs. Delete
  
- **Transactions**
  - COMMIT for saving changes
  - ROLLBACK for reverting changes
  - Transaction control

### **4. Joins and Relationships** 🔗
Combining data from multiple tables
- **INNER JOIN:** Records with matches in both tables
- **LEFT JOIN:** All records from left table + matching right
- **RIGHT JOIN:** All records from right table + matching left
- **FULL OUTER JOIN:** All records from both tables
- **CROSS JOIN:** Cartesian product of tables
- **Self Joins:** Joining table with itself
- **Multiple Joins:** Complex multi-table queries

### **5. Advanced Queries** 🚀
Complex data analysis
- **GROUP BY:** Aggregating data
  - Grouping by single and multiple columns
  - Statistical summaries by group
  
- **HAVING:** Filtering grouped data
  - Post-aggregation filtering
  - Complex group conditions
  
- **Subqueries and Nested Queries**
  - Scalar subqueries
  - Correlated subqueries
  - IN and EXISTS operators
  
- **Window Functions**
  - ROW_NUMBER() for ranking
  - PARTITION BY for grouped analysis
  - Running totals and moving averages
  
- **Common Table Expressions (CTEs)**
  - WITH clauses for readability
  - Recursive CTEs
  - Multiple CTEs in one query

### **6. Aggregation Functions** 📊
Summarizing data
- **COUNT():** Record count (with NULL handling)
- **SUM():** Total of numeric values
- **AVG():** Average values
- **MIN() / MAX():** Minimum and maximum values
- **STRING_AGG():** Concatenating strings
- **STDDEV() / VARIANCE():** Statistical functions

### **7. Indexing and Performance** ⚡
Optimizing database operations
- Index types and strategies
- Query optimization
- Execution plans
- Performance tuning tips

### **8. Views and Stored Procedures** 🔧
Advanced database objects
- Creating and managing views
- Stored procedures for reusable logic
- User-defined functions
- Triggers for automatic actions

---

## 📊 Common SQL Patterns

```sql
-- Finding duplicates
SELECT column, COUNT(*) FROM table GROUP BY column HAVING COUNT(*) > 1;

-- Ranking rows
SELECT *, ROW_NUMBER() OVER (PARTITION BY category ORDER BY value DESC) AS rank;

-- Year-over-year comparison
SELECT YEAR(date), COUNT(*) FROM sales GROUP BY YEAR(date);
```
- AVG(): Average values
- MIN() and MAX(): Extreme values

## 🎯 Key Concepts

### Data Types
- Numeric (INT, FLOAT, DECIMAL)
- String (VARCHAR, TEXT, CHAR)
- Date/Time (DATE, TIME, TIMESTAMP)
- Boolean (BIT, BOOLEAN)

### Constraints
- NOT NULL: Required fields
- UNIQUE: Prevent duplicates
- PRIMARY KEY: Unique identifier
- FOREIGN KEY: Referential integrity
- CHECK: Value validation
- DEFAULT: Default values

## 💻 Practical Applications

- Business intelligence and analytics
- Data warehousing
- Customer relationship management (CRM)
- Financial reporting
- Inventory management
- Log analysis and monitoring

## 🗄️ Popular SQL Databases

- **PostgreSQL:** Open-source, powerful
- **MySQL:** Widely-used, reliable
- **SQLite:** Lightweight, embedded
- **SQL Server:** Enterprise-grade (Microsoft)
- **Oracle Database:** Large-scale enterprise

## 📖 How to Use This Module

1. Start with basic SELECT queries
2. Learn filtering and WHERE clauses
3. Master JOIN operations for combining tables
4. Explore aggregation with GROUP BY
5. Practice with real datasets
6. Optimize queries for performance

## 🔧 Tools & Environment

### Development Tools
- **SQL Clients:** DBeaver, pgAdmin, MySQL Workbench
- **Online Platforms:** SQLFiddle, LeetCode SQL
- **IDEs:** VS Code with SQL extensions

### Best Practices
- Use descriptive table and column names
- Index frequently queried columns
- Write readable, commented queries
- Use parameterized queries to prevent SQL injection
- Optimize queries for performance
- Backup databases regularly

## 🔗 Related Modules

- Data Analysis with Pandas
- Machine Learning (data preparation)
- Business Intelligence and Analytics

## 📝 Common SQL Patterns

```sql
-- Basic SELECT with filtering
SELECT column1, column2 FROM table WHERE condition;

-- JOIN example
SELECT * FROM table1 JOIN table2 ON table1.id = table2.id;

-- Aggregation
SELECT COUNT(*), AVG(salary) FROM employees GROUP BY department;

-- Subquery
SELECT * FROM employees WHERE salary > (SELECT AVG(salary) FROM employees);
```

---

**Last Updated:** 2026  
**Difficulty Level:** Beginner to Intermediate  
**Prerequisites:** Basic database concepts helpful
