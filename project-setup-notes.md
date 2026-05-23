# Server Setup Notes

## EC2 Details

- Ubuntu Server 24.04
- AWS EC2 t2.micro

## Installed Utilities

- git
- wget
- curl
- unzip
- vim
- net-tools

## SSH Connection Successful

# Nginx Setup Notes

## Installed Nginx

Commands used:

- sudo apt install nginx -y
- sudo systemctl start nginx
- sudo systemctl enable nginx

## Website Directory

/var/www/html

## Log Files

Access Logs:
/var/log/nginx/access.log

Error Logs:
/var/log/nginx/error.log
