# apache_fdd
## Install Apache
```
sudo apt update
sudo apt install apache2
```

## Download this repository
```
git clone https://github.com/fengchenLBL/apache_fdd.git
cd ./apache_fdd
```

## Create a simple file server
```
sudo mkdir /var/www/fdd/
sudo cp ./index.txt /var/www/fdd/index.html
sudo cp ./fdd.conf /etc/apache2/sites-available/
sudo a2ensite fdd.conf
sudo systemctl reload apache2
```

## Create a symbolic link of current folder (e.g. this repository) under `/var/www/fdd/data`
```
sudo ln -s $(pwd) /var/www/fdd/data
```
## View/Download the shared data using web browser
URL: [data.localhost](http://data.localhost:8008)
