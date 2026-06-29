# Individual Assignment II: Oracle Pluggable Database (PDB) Administration

## 1. Assignment Overview
This assignment demonstrates the practical implementation of Oracle Multitenant Architecture, focusing on creating, managing, and deleting Oracle Pluggable Databases (PDBs), along with configuring dedicated database users and granting administrative privileges.

## 2. Oracle Environment
- *Oracle Version Used:* Oracle Database 21c Express Edition Release 21.0.0.0
- *Operating System:* Windows 10
- *Tools Used:* SQL*Plus, Command Prompt, GitHub

## 3. Task Documentation
### Task 1: Create and Configure a New Pluggable Database (PDB)
- Successfully created a persistent pluggable database named mo_pdb_308362025.
- Opened the PDB status to read-write mode.
- Switched session containers and created a local user named mohamed_plsqlauca_308362025 with full DBA/administrative privileges.
- Verified connection using the newly created credentials.

### Task 2: Create and Delete a Temporary PDB
- Created a temporary pluggable database named mo_to_delete_pdb_308362025.
- Verified its implicit initial closure state and securely dropped the temporary database alongside its respective datafiles.

## 4. Challenges and Solutions
- *Issue Encountered:* Faced error ORA-65005: missing or invalid file name pattern during the initial database creation process due to standard relative seed path conversions.
- *Solution Applied:* Explicitly resolved this obstacle by specifying the absolute internal file system paths mapping directly to the host storage environment.

## 5. Lessons Learned
Gained deep practical insight into multi-tenant container file conversion rules, dynamic session management, system privilege assignment policies, and repository structure tracking.

## 6. Integrity Statement
"I confirm that this assignment represents my own practical work, screenshots, and documentation. All external resources consulted have been properly acknowledged."
