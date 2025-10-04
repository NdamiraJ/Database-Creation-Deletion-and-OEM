## How to Enable Oracle Enterprise Manager (OEM)

Step 1: Connect to Your CDB as SYSDBA

Tool: SQL Developer

Use your existing connection to the FREE container database as:

Username: sys

Role: SYSDBA

Service name: FREE

Step 2: Enable HTTPS Port for OEM

Tool: SQL Developer

Run this command to activate OEM on port 5500:

sql
EXEC DBMS_XDB_CONFIG.SETHTTPSPORT(5500);
This tells Oracle to start listening for OEM traffic on that port.

Step 3: Restart the Listener

Tool: CMD

cmd
lsnrctl stop
lsnrctl start

# This refreshes the listener so it recognizes the new OEM configuration.

Step 4: Test the Connection Again

Tool: Browser

Try accessing:

Code
https://localhost:5500/em

