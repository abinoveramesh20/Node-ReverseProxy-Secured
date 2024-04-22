# Node-ReverseProxy in Apache-Secured
 Create a node app 
 1. npm init -y
 2. npm install
 3. Copy the  config file /etc/apache2/sites-available/000-default.conf as /etc/apache2/sites-available/my-node-app.conf
 4. Inside the my-node-app.conf uncomment the Servername your_domain also add the line
        ProxyPreserveHost On
        ProxyPass / http://13.233.253.32:8000/
        ProxyPassReverse / http://13.233.253.32:8000/
5. Now hit your domain along with port no. (127.0.0.1:8000)
6. After that Secure connection refer https://www.digitalocean.com/community/tutorials/how-to-secure-apache-with-let-s-encrypt-on-ubuntu

![ezcv logo](![Uploading Screenshot from 2024-04-22 17-50-15.png…]())


