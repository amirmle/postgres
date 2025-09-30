
    sudo -i -u  postgres
enter postgres env

    psql 
    -> postgres=#

create new db, user and grand privileges

    CREATE DATABASE mydb;
    CREATE USER myuser WITH ENCRYPTED PASSWORD 'mypassword';
    GRANT ALL PRIVILEGES ON DATABASE mydb TO myuser;
    
    \ist
    \l
    \q 
    exit

switch betwen databases

    \c mydb

list of all tables in current db

    \dt

list of all tables + views + other objects

    \d

structure of a table

    \d tablename

manage users

    \du
    \du username

command on terminal without exit from postgres 

    \! ls

man for all postgres commands

    \?


connect with new user

    psql -U myuser -d mydb -h localhos

