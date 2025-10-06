# Pl-assignment-2--Divince_cyusa

# Oracle Pluggable Database (PDB) Assignment  
**Student Name:** Divince Cyusa 

**Student ID:** 27516 


## Task 1: PDB Creation:
**Course:**  PL/SQL 

```
CREATE PLUGGABLE DATABASE plsql_class2025db
ADMIN USER divince_plsqlauca_27516 IDENTIFIED BY admin
FILE_NAME_CONVERT = ('C:\app\CYUSA\product\21c\oradata\XE\pdbseed','C:\app\CYUSA\product\21c\oradata\XE\XEPDB1\plsql_class2025db');

```
## Task 2: PDB Creation and Deletion for Temporary_pdb:
```
CREATE PLUGGABLE DATABASE di_plsqlauca_27516
ADMIN USER pl IDENTIFIED BY admin
FILE_NAME_CONVERT = ('C:\app\CYUSA\product\21c\oradata\XE\pdbseed','C:\app\CYUSA\product\21c\oradata\XE\XEPDB1\di_plsqlauca_27516');

 	step 1: ALTER PLUGGABLE DATABASE di_plsqlauca_27516 CLOSE;
	step 2: DROP PLUGGABLE DATABASE di_plsqlauca_27516 INCLUDING DATAFILES;
```

## Task 3: OEM Configuration: Set up Oracle Enterprise Manager (OEM) and took a screenshot of the dashboard showing the CDB and PDBs.

Screenshots:

Screenshot 1: PDB Creation screenshots/pdb1_creation.png

Screenshot 2: PDB Creation screenshots/pdb2_creation.png

Screenshot 3: PDB Creation screenshots/pdb2_deletion.png

Screenshot 4: OEM dabshoard screenshots/OEM_Dashboard.png


## Issues Encountered:

OEM Visibility Issue: The PDBs were not showing initially. Resolved by ensuring that the PDBs were in the open state.

ORA-01109 Error: Encountered when trying to delete a PDB that was not closed. Resolved by closing the PDB before deletion.

