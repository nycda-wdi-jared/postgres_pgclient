# First day of Postgres

<h1>Installation</h1>

1. Download Postgres
	* https://www.codementor.io/devops/tutorial/getting-started-postgresql-server-mac-osx
	* This is to download the software to run a separate server that connects to a postgres database

2. Download Postico
	* https://eggerapps.at/postico/
	* This is the ui in which you will be available to view the data in your database
	* This connects to your database server

3. Go through the installation process on both of those. Pick the most standard options.
4. Test out postgres in the terminal by typing ```postgres -V```
5. Next, type in these commands in the terminal:

	```psql -h localhost```

	```createdb testdb```

	```psql -c "CREATE USER admin WITH PASSWORD '';"```

6. Log into postico. Should like this:
![Alt text](https://github.com/nycda-wdi-jared/first_day_postgres/blob/master/postico_login.png)
	* I have no password, as that is how I set it up on postico
	* That's the login name I set up through the command i ran before
	* Port 5432 and a host of localhost is conventional.

7. Click on ```connect```, and if you get through without a problem, then you are ready to start creating tables and saving data

<h1>Installation/Postico Troubleshooting Websites</h1>
https://stackoverflow.com/questions/19828385/pgconnectionbad-could-not-connect-to-server-connection-refused

https://stackoverflow.com/questions/14564644/postgres-password-authentication-fails

https://www.codementor.io/devops/tutorial/getting-started-postgresql-server-mac-osx

https://www.a2hosting.com/kb/developer-corner/postgresql/managing-postgresql-databases-and-users-from-the-command-line

https://stackoverflow.com/questions/18715345/how-to-create-a-user-for-postgres-from-the-command-line-for-bash-automation

https://stackoverflow.com/questions/17633422/psql-fatal-database-user-does-not-exist

https://stackoverflow.com/questions/18715345/how-to-create-a-user-for-postgres-from-the-command-line-for-bash-automation

