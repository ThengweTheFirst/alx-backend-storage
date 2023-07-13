# 0x00. MySQL Advanced

This is a project focused on advanced concepts of MySQL and SQL. The goal of this project is to enhance your understanding and proficiency in working with MySQL databases, including creating tables with constraints, optimizing queries with indexes, implementing stored procedures, functions, views, and triggers.

## Authors
- Guillaume Plessis, Senior Cloud & System Engineer at WeWork
- Guillaume, CTO at Holberton school

## Project Schedule
- Start: Jul 12, 2023, 6:00 AM
- End: Jul 14, 2023, 6:00 AM
- Checker Release: Jul 12, 2023, 6:00 PM
- Auto Review: Will be launched at the deadline

## Concepts
In this project, you will explore the following concepts:
- Advanced SQL

## Resources
Read or watch the following resources:
- [MySQL cheatsheet](https://devhints.io/mysql)
- [MySQL Performance: How To Leverage MySQL Database Indexing](https://www.digitalocean.com/community/tutorials/mysql-performance-leverage-indexing)
- [Stored Procedure](https://dev.mysql.com/doc/refman/5.7/en/stored-procedures.html)
- [Triggers](https://dev.mysql.com/doc/refman/5.7/en/triggers.html)
- [Views](https://dev.mysql.com/doc/refman/5.7/en/views.html)
- [Functions and Operators](https://dev.mysql.com/doc/refman/5.7/en/functions.html)
- [Trigger Syntax and Examples](https://dev.mysql.com/doc/refman/5.7/en/trigger-syntax.html)
- [CREATE TABLE Statement](https://dev.mysql.com/doc/refman/5.7/en/create-table.html)
- [CREATE PROCEDURE and CREATE FUNCTION Statements](https://dev.mysql.com/doc/refman/5.7/en/create-procedure.html)
- [CREATE INDEX Statement](https://dev.mysql.com/doc/refman/5.7/en/create-index.html)
- [CREATE VIEW Statement](https://dev.mysql.com/doc/refman/5.7/en/create-view.html)

## Learning Objectives
By the end of this project, you should be able to explain the following topics without relying on external resources:

### General
- Creating tables with constraints
- Optimizing queries by adding indexes
- Implementing stored procedures and functions in MySQL
- Implementing views in MySQL
- Implementing triggers in MySQL

## Requirements
### General
- All files will be executed on Ubuntu 18.04 LTS using MySQL 5.7 (version 5.7.30)
- All files should end with a new line
- All SQL queries should have a comment just before them (i.e., syntax above)
- All files should start with a comment describing the task
- All SQL keywords should be in uppercase (e.g., SELECT, WHERE...)
- Include a README.md file at the root of the project folder
- The length of your files will be tested using `wc`

### Additional Information
Comments for your SQL file:
```
$ cat my_script.sql
-- 3 first students in the Batch ID=3
-- because Batch 3 is the best!
SELECT id, name FROM students WHERE batch_id = 3 ORDER BY created_at DESC LIMIT 3;
$
```

Use "container-on-demand" to run MySQL. Ask for a container with the following specifications:
- Ubuntu 18.04
- Python 3.7

You can connect to the container via SSH or the WebTerminal.

In the container, start MySQL before working with it:
```
$ service mysql start
 * MySQL Community Server 5.7.30 is started
$
```

To import a SQL dump, follow these steps:
```
$ echo "CREATE DATABASE hbtn_0d_tvshows;" | mysql -uroot -p
Enter password:
$ curl "https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/274/hbtn_0d_tvshows.sql" -s | mysql -uroot -p hbtn_0d_tvshows
Enter password:
$ echo "SELECT * FROM tv_genres" | mysql -uroot -p hbtn_0d_tvshows
Enter password:
id  name
1   Drama
2   Mystery
3   Adventure
4   Fantasy
5   Comedy
6   Crime
7   Suspense
8   Thriller
$
```

In the container, the credentials are `root/root`.

**Note:** This is a sample README.md file for the given project. You may need to modify or add more information based on the actual project requirements and guidelines.
