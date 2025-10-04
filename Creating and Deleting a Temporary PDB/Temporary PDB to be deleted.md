## Creating a temporary PDB to be deleted 

CREATE PLUGGABLE DATABASE jos_to_delete_pdb_27838
ADMIN USER josias_plsqlauca_27838 IDENTIFIED BY Auca
ROLES=(DBA)
FILE_NAME_CONVERT=('C:\APP\ADMIN\PRODUCT\23AI\ORADATA\FREE\PDBSEED\',
                   'C:\APP\ADMIN\PRODUCT\23AI\ORADATA\FREE\jos_to_delete_pdb_27838\');

## Deleting a temporary PDB created

DROP PLUGGABLE DATABASE jos_to_delete_pdb_27838 INCLUDING DATAFILES;

Screenshots:

![alt text](<PDB to be deleted.png>)

![alt text](<Deleted tempory PDB created.png>)