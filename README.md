# Linux Server Configuration

## Server Info
* IP address : 18.219.133.44
* SSH port : 2200
* App Home : [http://18.219.133.44/catalog/](http://18.219.133.44/catalog/)

## Issues
The web app can only use Github OAuth

## Summary of configurations
1. update system software
2. set sshd to listen on 2200, disable password and root login
3. using ufw to only allow incoming connection from ssh(2200), http(89), ntp(123)
4. add a user named grader, give sudo privilege, and setup rsa key for ssh
5. clone my Catalog App, setup apache2 and postgresql, and configure wsgi