# Your Project Name
This is a startup guide for setting up your project.

> Don't upload sensitive data like credit card / bank account details and any kind of secret key like aws private key, sms gateway, payment gateway, database credential etc.

## Prerequiestes
* Node 7.9.0+
* Npm 5.0 +
* MongoDB (Version)
* Apache (Version)
* Nginx (Version)
* Mysql (Version)
* MongoDB (Version)

## Getting Started
You can download this repo or clone using below command. (folder-name will be project folder in which you want to start your project).
```
git clone https://github.com/chiragvbacancy/test.git <folder-name>
```
or from **Download Zip**
```
https://github.com/chiragvbacancy/test.git
```
## Project Setup
Once you clone or download project go into you folder

>now rename **.env.example** file to **.env** file
>Add related settings data into .env file (All database config and other important and private data will be stored in .env file only)

## Installing Dependencies
```
> npm install     (this will install all node dependencies)
```

## Database Config Setup
Create new database (let's say i'm going to use mysql and my database name is **test**).
so in my **.env** file will set below parameters.
```
DB_HOST_DEV=localhost
DB_USER_DEV=root
DB_PASSWORD_DEV=root
DB_NAME_DEV=test
DB_PORT_DEV=3306
```
### Database Migration and Seeders run
After creating database and updating .env file run below commands
```
> node_modules/.bin/sequelize db:migrate
> node_modules/.bin/sequelize db:seed:all
> For More imformation about database: http://docs.sequelizejs.com/manual/tutorial/migrations.html
```
## Schedulers or Cron jobs
List out Schedulers or cron jobs details (Start time, location etc.)

## Project Run
`node app.js` to run your project 
>Everythig is setup and you are good to go now. Happy Coding :)
