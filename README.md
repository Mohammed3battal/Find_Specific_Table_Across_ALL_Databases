# Find_Specific_Table_Across_ALL_Databases

**Description**:
This script uses sp_MSforeachdb to loop through all databases on the SQL Server instance and check whether a specific table (default: table1) exists. If the table is found in any database, the script prints the database name.

What It Does:
Iterates over all user/system databases
Executes a check for the existence of table1 using INFORMATION_SCHEMA.TABLES
Prints the name of each database where the table exists

**Use Case**:
Find where a table is accidentally duplicated across databases
Track down legacy or temp tables after a migration
Validate schema distribution in multi-tenant or shared environments
