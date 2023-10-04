### Prerequisites
Windows Tools
Install chocolatey from the instructions given in the link below.
https://chocolatey.org/docs/installation
Run all the below commands on Powershell (Open Powershell as Admin)
choco install virtualbox --version=7.0.8 -y
choco install vagrant --version=2.3.4 -y
choco install git -y
choco install corretto11jdk -y
choco install maven -y
choco install awscli -y
choco install intellijidea-community -y
choco install vscode -y
choco install sublimetext3.app -y



JDK 11
Maven 3 or later
MySQL 5.6 or later
Technologies
Spring MVC
Spring Security
Spring Data JPA
Maven
JSP
MySQL
Database
### Here,we used Mysql DB MSQL DB Installation Steps for Linux ubuntu 14.04:

$ sudo apt-get update
$ sudo apt-get install mysql-server
Then look for the file :

/src/main/resources/accountsdb
accountsdb.sql file is a mysql dump file.we have to import this dump to mysql db server
mysql -u <user_name> -p accounts < accountsdb.sql
