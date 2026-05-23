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

# Node Exporter Setup

## Purpose

Collect Linux system metrics for Prometheus.

## Installed Version

v1.9.1

## Metrics Endpoint

http://SERVER_IP:9100/metrics

## Important Commands

Start Service:
sudo systemctl start node_exporter

Check Status:
sudo systemctl status node_exporter

View Metrics:
curl localhost:9100/metrics

# Prometheus Setup

## Installed Version

v3.4.1

## Metrics UI

http://SERVER_IP:9090

## Config File

/etc/prometheus/prometheus.yml

## Monitored Targets

- localhost:9090
- localhost:9100

## Important Commands

Check Status:
sudo systemctl status prometheus

Restart:
sudo systemctl restart prometheus
