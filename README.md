1. Connect database to python:

SQL Server connection details<br/>
DB_CONFIG = {<br/>
    "server": "Server Name",<br/>
    "database": "LARCarRental"<br/>
}<br/>

- Change the 'Server Name' to the SQL server name
- It is Windows Authentication

2. Run the Application<br/>
- Run the python code and a website link will appear.<br/>
- Click on the link to bring you to the website.

3. Login<br/>
- The username is "admin"<br/>
- The password is "password"

4. the server certificate query
USE master;
BACKUP CERTIFICATE MyServerCert
TO FILE = 'C:\TDE_backups\MyServerCert.cer'
WITH PRIVATE KEY (
    FILE = 'C:\TDE_backups\MyServerCert.pvk',
    ENCRYPTION BY PASSWORD = 'Pa$$w0rd'
);
