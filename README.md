# README
This is a twitter clone practice app using react and ruby on rails
To start in local use rails s

Pre-requisites:
1. Ruby and rails installed
ruby --version
ruby 2.7.0p0 (2019-12-25 revision 647ee6f091) [x86_64-linux-gnu]

rails --version
Rails 5.2.6.2

2. postgresql installed
psql --version
psql (PostgreSQL) 12.9 (Ubuntu 12.9-0ubuntu0.20.04.1)

3. If new database is installed, follow the steps to create default db:
3.1
sudo su postgres psql #1 logged in as default user and login into the postgres interactive terminal
CREATE user <username from database.yml file> with password '<value for ALEX_PG_PASS>'; #create new user
alter user <username from database.yml file> with superuser; #Make the user your have just created a superuser
\du #View a list of roles while in the postgres interative terminal. Make sure it lists superuser
\q #quit

3.2
rake db:create ALEX_PG_PASS='<your password from pg setup>'    
