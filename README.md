# blue-green
Blue/Green deployments using Traefik

# Generate a self-signed certificate for MS SQL Server
[Reference](https://learn.microsoft.com/en-us/sql/linux/sql-server-linux-docker-container-security?view=sql-server-ver16#encrypt-connections-to-sql-server-linux-containers)
1. Create a self-signed certificate for MS SQL Server and set the permissions
```
openssl req -x509 -nodes -newkey rsa:2048 -subj '/CN=db.docker.localhost' -keyout mssql.key -out mssql.pem -days 365
```
