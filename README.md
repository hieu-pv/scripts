# Installation
* First, download the package using Composer:
```
composer global require nf/scripts
```
* Make sure to place the $HOME/.composer/vendor/bin directory (or the equivalent directory for your OS) in your $PATH so the laravel executable can be located by your system.
* Update your information by run update command, we do it whenever you want to change your information
```
nfupdate
```
# Command

##### Set ipv6off
Disable ipv6
```
setv6off [-t|--type]
```
-t|--type (optional) Wi-Fi or Ethernet
##### List all your databases
The result is same with "show databases" query
```
dbshow
```
##### Create new database
```
dbcreate {database_name} [-d|--drop]
```
-d|--drop(optional) drop your existing database and create new one
##### Dump database
```
dbdump {database_name} {relative_path_to_your_sql_file} [-d|--drop] [-c|--create] [-u|--user] [-p|--password]
```
-d|--drop (optional) drop your existing database before dump

-c|--create (optional) create new database before dump

-u|--user (optional) MySQL username if you want to run this command with given username

-p|--password (optional) MySQL password if you want to run this command with given password
##### Edit hosts file (Mac only)
Open your hosts file 
```
edithost
```
