# AWS Three-Tier Architecture Commands

## Update Packages

```bash
sudo dnf update -y
```

## Install Apache Web Server

```bash
sudo dnf install httpd -y
```

## Start Apache Service

```bash
sudo systemctl start httpd
```

## Enable Apache Service

```bash
sudo systemctl enable httpd
```

## Check Apache Status

```bash
sudo systemctl status httpd
```

## Create Web Page

```bash
echo "Hello from the Application Tier!" > /var/www/html/index.html
```

## Verify Website

```bash
curl localhost
```

## Git Commands

```bash
git status
git add .
git commit -m "Completed AWS Three-Tier Architecture Project"
git push origin main
```