Clone the Project 

1. bundle install
2. rails s 

How to setup POSTGRES DB

If you have password error then do this 
1. Go to -> C:\Program Files\PostgreSQL\12\data
2. Change files permissions
3. Open file pg_hba.conf and replace mothods with Trust 

# TYPE  DATABASE        USER            ADDRESS                 METHOD

# IPv4 local connections:
host    all             all             127.0.0.1/32            trust
# IPv6 local connections:
host    all             all             ::1/128                 trust
# Allow replication connections from localhost, by a user with the
# replication privilege.
host    replication     all             127.0.0.1/32            trust
host    replication     all             ::1/128                 trust

_______________________________________________________________________________

First of all add path of POSTGRES

Add to Enviroment Path 
1. C:\Program Files\PostgreSQL\12\bin
2. C:\Program Files\PostgreSQL\12\lib

Now you can run POSTGRES QURIES through CMD on windows

Open CMD and type 
1. psql -U postgres postgres
2. create role salman login; // have all the permission without the passowrd
3. \du TO Check existing roles

For more info check this 
https://www.enterprisedb.com/postgres-tutorials/how-create-postgresql-database-and-users-using-psql-and-pgadmin