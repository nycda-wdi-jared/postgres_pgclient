# Heroku Details For Node/Postgres

<h2>Heroku</h2>

* Be sure that your current directory is connected to a git repo
* Run ```heroku create```
* Run ```heroku addons:create heroku-postgresql:hobby-dev```
* In this case, we have some pre-populated data in our database, so we want have that pre-populated data in heroku as well. To do that, run this command: ```pg_dump dbname > outfile```
	* Have your outfile named something like 'backup.sql'
	* My command for this app would look like this ```pg_dump iTunes_crud > backup.sql```
* Run ```heroku pg:psql --app <Heroku App Name> DATABASE < backup.sql```
	* Be sure to have a schema.sql file in the root directory of your folder
	* Be sure to define all of the schema to create your tables, as heroku does not automatically that for you
	* If you push up to heroku without running this command, then your database will have no tables
	* You can also sign into the database through postico and run your schema there
* Run ```heroku config``` to see the env variable just added to the Heroku environment
* Resource: https://devcenter.heroku.com/articles/heroku-postgresql

<h2>More</h2>

* You can connect to this database through the credentials they give you
* You can see a breakdown of the credentials if you go to your app's page on heroku and find the database option
![postgres image one](https://github.com/nycda-wdi-jared/pg_express_crud_guestbook/blob/master/github_images/first.png?raw=true "Postgres Example")
![postgres image two](https://github.com/nycda-wdi-jared/pg_express_crud_guestbook/blob/master/github_images/second.png?raw=true "Postgres Example")