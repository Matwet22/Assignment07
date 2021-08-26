# ------------------------------------------------- #
# Title: Assignment07
# Description: Functions/UDFs
# ChangeLog: (Who, When, What)
# MWaring,8.25.2021,Created Script
# ------------------------------------------------- #


# Functions/UDFs

## Introduction
### This paper will discuss SQL functions, including User Defined Functions, and their various types. SQL functions allow computations to be performed on fields from a table in a database. These are abstraction layers and have similarities to stored procedures and views. 

## User Defined Functions (UDFs) 

### User defined functions (UDFs), like views, are methods of abstraction that wrap around a select statement to return sets of data. They allow us to create our own functions and store them. Like views, UDFs can return a table. They may also return a single value. For simple queries, views are easy and preferable. When adding in complexity, UDFs may be a better option. Unlike views, UDFs also allow adding check constraints. 

### Functions return a single value, or a table of values. To return a table, the operator Returns (with an ‘s’) is used, followed by ‘Table’, then a select statement defines what fields will be included in the table. The returns operator allows us to choose the data type that will be returned by the function. 

## Scalar, Inline, and Multi-Statement Functions

### Scalar, inline, and multi-statement functions all take in parameters, processes, and returns a value or set of values. Scalar functions return a single value, rather than a table. They don’t have to have parameters but will always return a single value. 
Returned values can be any data type, float, integer, varchar, date, datetime, etc. The Return keyword will define the datatype to be returned. Scalar functions require a two part name when invoked, ex dbo.FunctionX. Inline functions are very similar to views, more so than scalar or multi-statement functions. They use one select statement and could be considered single statement functions. Multi-Statement Functions are very similar to inline table functions but return variable data and always use Begin and End clauses. Unlike inline functions, the data type needs to be set for multi statement functions. 

## Conclusion

### SQL functions offer a robust set of options for making calculations on data from tables. We may choose from a set of built-in options or create our own user defined functions. User defined functions can result in tables and have similarities to views. They provide a layer of abstraction from a database, much like views and stored procedures. User defined functions allow for complex computations, and can be scalar, inline, or multi statement.
