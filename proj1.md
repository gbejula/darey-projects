# PROJECT 1: LAMP STACK IMPLEMENTATION

> WEB STACK IMPLEMENTATION (LAMP STACK) IN AWS

- Create AWS account and set up ubuntu server

- Connected to the EC2 instance.

- Navigated to download to copy for the **.pem** file

> ## Step 1 - Installing Apache and updating the linux

- Install apache on ubuntu instance using the command below:

```
sudo apt update
sudo apt install apache2
sudo systemctl status apache2
```

![apache installed](proj1/apache2-running.png)

- Check apache in the console

![apache in console](proj1/apache2-curl-check.png)

- Check apache in the browser

![apache in browser](proj1/apache2-on-browser.png)

> ## Step 2 - Install MySQL

- To install mysql

```
sudo apt install mysql-server
sudo mysql
```

![install mysql](proj1/mysql-running.png)

- Changed mysql password

![mysql password changed](proj1/new-password-mysql.png)

> ## Step 3 - Install PHP

- To install these 3 packages at once, run

```
sudo apt install php libapache2-mod-php php-mysql
php -v
```

![php installed](proj1/php--installed.png)

> ## Step 4 - Creating a virtual host for your website using Apache

```
sudo mkdir /var/www/projectlamp
sudo chown -R $USER:$USER /var/www/projectlamp
sudo vi /etc/apache2/sites-available/projectlamp.conf
```

![make a directory and change ownership](proj1/sensitive-info-removed.png)
