## Assignment Overview

This assignment covers the creation and deletion of Pluggable Databases (PDBs), configuration of Oracle Enterprise Manager (OEM), and documentation of troubleshooting steps.

## Task 1: Creating a New Pluggable Database (PDB)

- **PDB Name**: `jos_pdb_27838`
- **Username**: `josias_plsqlauca_27838`
- **Password**: `Auca`
- **Purpose**: This account stores all class work and exercises.

Find screenshots in the screenshot folder [text](Sceenshots) 


## Task 2: Create and Delete a PDB

- **PDB Name**: `jos_to_delete_pdb_27838`
- **Action**: Created and then deleted using SQL Developer and CMD
- **Command Used**:
  ```sql
  DROP PLUGGABLE DATABASE jos_to_delete_pdb_27838 INCLUDING DATAFILES;

## Task 3: Oracle Enterprise Manager (OEM)

Attempted Access: https://localhost:5500/em

- Result: OEM returned “Not Implemented” error

- Cause: OEM Express not supported or mapped in Oracle Free 23c

- Adaptation: Used SQL Developer queries to simulate OEM functionalit

## Issues & Solutions

- Issue: OEM Not Accessible
- Cause: Endpoint /em not supported
- Solution: Enabled HTTPS port, restarted listener, used SQL Developer views


📄 Notes

All tasks were completed using SQL Developer, CMD, and PowerShell

Screenshots and markdown documentation are organized in the assignment folder

Troubleshooting steps demonstrate resilience and technical depth