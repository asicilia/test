Map-On
======
**A web-based editor for visual ontology mapping**
Map-On is a graphical environment for ontology mapping which helps different kinds of users to carry out ontology mapping processes by establishing relations between the elements of a database and a domain ontology.

----------

Installation
-------------

#### Create the database

1. Create a database called 'mapon' and import tables from 'mapon_base_db.sql'
> CREATE DATABASE mapon;
> mysql --user=<database_user> --password=<database_password> mapon < mapon_base_db.sql

Note: Sql file are located in 'application/config/mapon_base_db.sql'

#### Framework configuration

1. Rename the files 'config.dist.php' and 'database.dist.php' to 'config.php' and 'database.php'
> sudo cp application/config/config.dist.php application/config/config.php 
> sudo cp application/config/database.dist.php application/config/database.php 

2. Modify base_url variable from 'application/config/config.php'
> $config['base_url'] = 'http://localhost/<project_path>';

3. Modify database credentials from 'application/config/database.php'
> $db['default']['username'] = 'database_username';
> $db['default']['password'] = 'database_password';
