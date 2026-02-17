# oracle_pdb_ass_II_-28752-_-Shima-
course:Database Development with PL\SQL
STUDENT NAME:SHIMA GISELE
STUDENT ID:28752

## OVERVIEW OF THE ASSIGNMENT
This assignment focuses on practical implementation of Oracle Multitenant Architecture, specifically the creation and management of Pluggable Databases (PDBs).

Through this assignment, I practiced:
	•	Creating and opening a Pluggable Database (PDB)
	•	Creating a user inside a PDB
	•	Creating and deleting a temporary PDB
	•	Accessing and verifying configurations using Oracle Enterprise Manager (OEM)
	•	Documenting technical work professionally using GitHub

 ## Oracle Environment Used
 Oracle Database Version:ORACLE 21C
 Operating System: WINDOWS 10
 Tools Used: SQL*PLUS, SQL DEVELOPER
 OEM Access: Web browser (localhost)
## Task 1: Create a New Pluggable Database
In this task,  created a new Pluggable Database following the exact naming conventions provided in the assignment instructions.
Steps Performed:
	1.	Connected to the Container Database (CDB) as SYSDBA.
   sqlplus / as sysdba
	2.	Created the PDB using the required naming format.
 CREATE PLUGGABLE DATABASE gisele_pdb_28752
   ADMIN USER gisele_plsqlauca_28752 IDENTIFIED BY shima 
   FILE_NAME_CONVERT=('pdbseed','gi_pdb_28752');
	3.	Created a user inside the PDB using the required naming convention.
 CREATE USER shima_plsqlauca_28752 IDENTIFIED BY shima;
	4.	Granted appropriate privileges to the user .
 GRANT CONNECT, RESOURCE TO shima_plsqlauca_28752;
 
 ## Task 2: Create and Delete a PDB
 For this task, created a temporary PDB and then completely removed it.

Steps Performed:
	1.	Created a temporary PDB using the specified naming format.
	CREATE PLUGGABLE DATABASE si_to_delete_pdb_28752
   ADMIN USER admin IDENTIFIED BY admin
   FILE_NAME_CONVERT=('pdbseed','si_to_delete_pdb_28752');
	2.	Closed the PDB before deletion.
 ALTER PLUGGABLE DATABASE si_to_delete_pdb_28752 CLOSE IMMEDIATE;
	3.	Dropped the PDB including its datafiles.
	DROP PLUGGABLE DATABASE si_to_delete_pdb_28752INCLUDING DATAFILES;

 ## Task 3: Oracle Enterprise Manager (OEM)
I configured and accessed Oracle Enterprise Manager through the browser.
Using OEM, I verified:
	•	The existence of my created PDB
	•	The successful deletion of the temporary PDB
	•	The overall Oracle environment status

All sources were properly cited.Implementations and analysis represent original work.No AI generated content was copied without attribution or adaptation.


<img width="543" height="113" alt="pluggable database" src="https://github.com/user-attachments/assets/c7bb6262-2369-4177-8d55-861698fd5193" />

<img width="854" height="453" alt="pic 2" src="https://github.com/user-attachments/assets/3d6ba1f8-7a29-4e72-a04a-ac6465b9ccc2" />

<img width="859" height="438" alt="pic 4" src="https://github.com/user-attachments/assets/ff5f240d-486d-483f-bc12-9b4467acb283" />

<img width="852" height="448" alt="pic 7" src="https://github.com/user-attachments/assets/6482d517-1faf-4b71-9e20-d4c996608b1a" />

<img width="946" height="403" alt="pic 8" src="https://github.com/user-attachments/assets/dca59125-3a8e-4337-aef4-e9a065453612" />




 




