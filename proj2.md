# PROJECT 2: LEMP STACK IMPLEMENTATION

> ## Step 1: Installing Nginx web server

- Create AWS account and set up ubuntu server

- Connect to the EC2 instance.

- Update the Ubuntu server and install nginx web server

```
sudo apt update
sudo apt install nginx
```

- Check the status of the Nginx web server to verify that nginx was successfully installed and is running as a service in Ubuntu, run:

`sudo systemctl status nginx`

- If it is green and running, then everything is working correctly – First Web Server is launched in the Cloud!

- To receive any traffic from the web server, open TCP port 80 which is the default port that web browsers use to access web pages in the internet.

- The web server is running and it can be accessed locally and from the Internet (Source 0.0.0.0/0 means ‘from any IP address’).

- To access it locally in our Ubuntu shell, run:

```
curl http://localhost:80
or
curl http://127.0.0.1:80
```

- To access the web server from the internet, open a web server and try to access the following url:

`http://<Public-IP-Address>:80`

- If you see following page, then your web server is now correctly installed and accessible through your firewall.

![nginx-in-the-browser](proj2/nginx-4m-browser.png)

> ## Step 2: Install MYSQL

- Run the following command in the terminal to install mysql

`sudo apt install mysql-server`

- Once the installation is finished, log in to the MYSQL console by typing:

`sudo mysql`

![mysql-installed](proj2/mysql-installed.png)

- Reset the password for mysql and set the password strenght

![mysql-set-password](proj2/mysql-set-name-password.png)

> ## Step 3 - Install PHP

- Install PHP using the command below:

`sudo apt install php-fpm php-mysql`
