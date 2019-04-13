# Devilbox Magento2 Instruction

|Linux|Windows|
|---|---|
|git clone https://github.com/cytopia/devilbox|Clone https://github.com/cytopia/devilbox to C:\devilbox with Git for Windows|
|cd devilbox<br>cp env-example .env|Copy C:\devilbox\env-example to C:\devilbox\.env|

Create a folder
mkdir ../workspace

Move `data` folder outside
mv data/ ../workspace/

Edit `.env` file
Set `TIMEZONE` to `Europe/Kiev`

Uncomment `#PHP_SERVER=7.1`
Comment `#PHP_SERVER=7.2`

Uncomment `HTTPD_SERVER=apache-2.4`
Comment `HTTPD_SERVER=nginx-stable`

Uncomment `MYSQL_SERVER=mysql-5.7`
Comment `MYSQL_SERVER=mariadb-10.3`

Replace `HOST_PATH_HTTPD_DATADIR=./data/www` to `HOST_PATH_HTTPD_DATADIR=../workspace/data/www`

Replace `MYSQL_ROOT_PASSWORD=` to `MYSQL_ROOT_PASSWORD=123123q`
