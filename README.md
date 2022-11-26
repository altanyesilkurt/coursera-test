# Enquire Al FinNews Portal 

                                                                        ## Requirements
## Docker 
                                                                        
 - [Docker Desctop](https://docs.docker.com/desktop/install/windows-install/)

## Install Postgres 12.5

 Run the commands:

```bash
docker pull postgres:12.5
docker run --name postgres -p 5432:5432 -e POSTGRES_USER=<POSTGRES_USER> -e POSTGRES_PASSWORD=<POSTGRES_PASSWORD> -p postgres:12.5
```

## Create Database Schema

Create Table. Run the command in the "create_table_script.sql" file.

## Ingestion

install python 3.10.8 (https://www.python.org/downloads/)

Run the command to install required libraries module in cron_job.py class:
```bash
pip install
```
install crontab and Run the command: 
```bash
sudo apt-get install cron
crontab -e
```
job will run in every 5 minutes. Add the following code on top and save:
```bash
*/5 * * * * python3 cron_job.py
```
run  the following commad
```bash
service cron start
```

## Api
Java version is 17.
Build and run project.
Default go to the link http://localhost/8080 

## UI Portal

install Node js v14.15.5
install Angular CLI. Run the command:
```bash
npm install –g @angular/cli@14.2.1
```

Running the portal ui is also easy. Just run the commands:

```bash
npm install
ng serve
```
This command will wait for build an serve ready, go to the link http://localhost/4200 



