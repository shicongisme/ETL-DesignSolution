# ETL Solution for AndresWorld

Designing and implementing an ETL solution to load a small portion of a data warehouse in SQL Server 2016 and tracking historical information using SSIS.

### Environment
* Microsoft SQL Server Management Studio
* Microsoft Visual Studio

### Tasks
1. Creating a staging area (an empty database warehouse) containing only the database schema `Scripts`.
2. Loading data from a flat file into a temporary AndresW OLTP database `Scripts`.
3. Adding more columns in the dimensions for SCD if they do not exist to track historical values `Scripts`.
4. Disabling single constraint in the data warehouse and at the end re-adding constraints `Scripts`.
5. Control flow view from SSIS.

<p align="center">
  <img width="500" src="Images/Fig1.jpg">
</p>

6. Data flow view from SSIS. The customer dimension is shaped from different sources. We have data coming from the database, data coming from a flat file, and more data through a temp table via a lookup (as well as defaulting data that we don't have).
7. SCD is implemented

<p align="center">
  <img width="500" src="Images/Fig2.jpg">
</p>
