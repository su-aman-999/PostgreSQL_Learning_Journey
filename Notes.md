# Installation

# 📌 5 Types of Commands in SQL

- DDL (Data Definition Language)
- DML (Data Manipulation Language)
- TCL (Transaction Control Language)
- DCL (Data Control Language)
- DQL (Data Query Language)

# 🏗️ Data Definition Language (DDL)

DDL commands database structure define/modify karte hain.
| Command | Description | Example |
| -------- | ---------------------------------------------- | --------------------------------------------- |
| CREATE | New database object create karta hai | `CREATE TABLE employees (id INT, name TEXT);` |
| ALTER | Existing structure modify karta hai | `ALTER TABLE employees ADD COLUMN age INT;` |
| DROP | Table ya object delete karta hai | `DROP TABLE employees;` |
| TRUNCATE | Table ke saare records delete karta hai (fast) | `TRUNCATE TABLE employees;` |

# ✏️ Data Manipulation Language (DML)

DML commands table ke data ko handle karte hain.

| Command | Description                      | Example                                                         |
| ------- | -------------------------------- | --------------------------------------------------------------- |
| INSERT  | New record add karta hai         | `INSERT INTO employees (id, name, age) VALUES (1, 'John', 30);` |
| UPDATE  | Existing data modify karta hai   | `UPDATE employees SET age = 31 WHERE id = 1;`                   |
| DELETE  | Specific record delete karta hai | `DELETE FROM employees WHERE id = 1;`                           |
| SELECT  | Data retrieve karta hai          | `SELECT * FROM employees;`                                      |

# 🔄 Transaction Control Language (TCL)

TCL commands transactions manage karte hain.
| Command | Description | Example |
| --------- | ---------------------------------- | ---------------- |
| BEGIN | Transaction start karta hai | `BEGIN;` |
| COMMIT | Changes save karta hai | `COMMIT;` |
| ROLLBACK | Changes undo karta hai | `ROLLBACK;` |
| SAVEPOINT | Transaction me point set karta hai | `SAVEPOINT sp1;` |

# 🔐 Data Control Language (DCL)

DCL user permissions control karta hai.
| Command | Description | Example |
| ------- | ------------------------- | --------------------------------------------- |
| GRANT | Permission deta hai | `GRANT SELECT, INSERT ON employees TO user1;` |
| REVOKE | Permission wapas leta hai | `REVOKE INSERT ON employees FROM user1;` |

# 🔍 Data Query Language (DQL)

DQL mainly data fetch karne ke liye use hota hai.
| Command | Description | Example |
| ------- | ----------------------- | ------------------------------------------------- |
| SELECT | Data retrieve karta hai | `SELECT name, age FROM employees WHERE age > 25;` |

# 💡 Pro Tip (Important for Beginners)

- Hamesha COMMIT aur ROLLBACK carefully use karo
- Pehle SELECT run karke data check karo
- Direct changes mat karo bina samjhe

# ⚔️ SQL vs NoSQL (Short Comparison)

## 📦 Data Storage

- **SQL** → Tables (rows & columns)
- **NoSQL** → JSON, key-value, graph, etc.

# 📊 Comparison Table

| Aspect          | SQL Databases                 | NoSQL Databases                |
| --------------- | ----------------------------- | ------------------------------ |
| Data Model      | Relational (Table-based)      | Non-relational                 |
| Structure       | Structured (rows & columns)   | Unstructured / Semi-structured |
| Schema          | Fixed                         | Flexible                       |
| Query Language  | SQL                           | JSON-like / different methods  |
| Scalability     | Vertical                      | Horizontal                     |
| ACID Compliance | Strong                        | Eventual consistency           |
| Use Case        | Complex queries, transactions | Big data, real-time apps       |
| Examples        | MySQL, PostgreSQL, Oracle     | MongoDB, Cassandra, Redis      |
| Performance     | Complex queries optimized     | Fast reads/writes              |
| Relationships   | Supports foreign keys         | No predefined relations        |
| Transactions    | Full support                  | Limited                        |

#
