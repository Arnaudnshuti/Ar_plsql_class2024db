# ar_plsql_class2024db - Oracle PL/SQL Class Activities

This repository contains SQL scripts and activities related to the Oracle PL/SQL class, focusing on the creation, management, and deletion of Pluggable Databases (PDBs) using Oracle 21c. The repository also includes tasks related to configuring Oracle Enterprise Manager (OEM) for monitoring and managing databases.

## Table of Contents
- [Overview](#overview)
- [Project Setup](#project-setup)
- [Tasks and Commands](#tasks-and-commands)
  - [Task 1: Creating a PDB](#task-1-creating-a-pdb)
  - [Task 2: Deleting a PDB](#task-2-deleting-a-pdb)
  - [Task 3: Configuring Oracle Enterprise Manager (OEM)](#task-3-configuring-oracle-enterprise-manager-oem)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

## Overview

The main objective of this project is to:
- Create and manage a Pluggable Database (PDB) with a specific format for username and password.
- Delete a PDB as per assignment requirements.
- Configure Oracle Enterprise Manager (OEM) to monitor and manage the database.

This repository contains all necessary SQL scripts, configurations, and screenshots to demonstrate the tasks carried out during the course.

## Project Setup

### Prerequisites
Before working on this repository, ensure you have the following:
- Oracle Database 21c or later installed
- Oracle SQL*Plus or another SQL tool
- Basic knowledge of PL/SQL and Oracle Database Management

### Cloning the Repository
To get started with the repository, clone it to your local machine:

```bash
git clone https://github.com/your_username/ar_plsql_class2024db.git
cd ar_plsql_class2024db
```

## Tasks and Commands

## Task 1: Creating a PDB
I created a Pluggable Database (PDB) named plsql_class2024db with a user ar_plsqlauca.

### SQL Command Used:
```sql
CREATE PLUGGABLE DATABASE plsql_class2024db
ADMIN USER ar_plsqlauca IDENTIFIED BY 123
FILE_NAME_CONVERT = ('C:\app\Administrator\product\21c\oradata\XE\', 'C:\app\Administrator\product\21c\oradata\plsql_class2024db\');
```

## Task 2: Deleting a PDB

After creating another PDB named ar_to_delete_pdb, I deleted it using the following SQL commands:

### SQL Command for deletion:
```sql
ALTER PLUGGABLE DATABASE ar_to_delete_pdb CLOSE IMMEDIATE;
DROP PLUGGABLE DATABASE ar_to_delete_pdb INCLUDING DATAFILES;
```

## Task 3: Configuring Oracle Enterprise Manager (OEM)

I configured Oracle Enterprise Manager (OEM) to manage the PDBs. 
After setting it up, I accessed the OEM dashboard for monitoring and management purposes.

## Screenshots

## PDB Creation:

![pdb_created(66)](https://github.com/user-attachments/assets/ba8fda20-73c7-41cc-a72a-020ab85d32c3)


## PDB Deletion:

![pdb_dropped(65)](https://github.com/user-attachments/assets/9ff6b15a-aec2-4357-b1c1-28deb25fe8c2)
## OEM Checking the host:
![checking hostt (68)](https://github.com/user-attachments/assets/4566d1d8-4149-4782-b5b0-41ec638515de)

## OEM Login_page:
![OEM_Login page (72)](https://github.com/user-attachments/assets/426ea00e-07e7-4096-9e9b-684e7e29eefd)


## OEM Dashboard:
![OEM_Login page (72)](https://github.com/user-attachments/assets/d925c561-ac1c-4b6f-8796-36f3606715d3)
## OEM Table Dashboard:
![OEM_Table dashboard (73)](https://github.com/user-attachments/assets/4fa98900-eafa-46fb-b5bf-c1f34c79336a)

## Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request with your improvements or suggestions.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT). You can freely use, copy, modify, and distribute this software, but please include a copy of this license in any distributions.

















