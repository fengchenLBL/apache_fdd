# apache_fdd
## Installing Apache
```
sudo apt update
sudo apt install apache2
```

## Creating a simple file server
```
sudo mkdir /var/www/fdd/
sudo cp ./index.html /var/www/fdd/
sudo cp ./fdd.conf /etc/apache2/sites-available/
sudo a2ensite gci.conf
sudo systemctl reload apache2
```
