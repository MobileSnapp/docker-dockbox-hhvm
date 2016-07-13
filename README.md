# NGINX-HHVM server container for Dockbox

[![forthebadge](http://forthebadge.com/images/badges/built-by-developers.svg)](http://www.mobilesnapp.com)

Dockbox helps you run your PHP development environment on Docker. It provides all the virtual development environments that you would normally need for your PHP development. Dockbox is a tool that controls Docker for you (using Docker Compose official commands).

## Usage

    $ docker run -d -p 80:80 mobilesnapp/dockbox-hhvm
    
With all the options:
 
    $ docker run -d -p 80:80 \
        -v /home/user/app:/var/www/site \
        mobilesnapp/dockbox-hhvm

-v [local path]:/var/www/site maps the container's webroot to a local path
-p [local port]:80 maps a local port to the container's HTTP port 80

With SSL options

    $ docker run -d -p 80:80 -p 443:443 \
        -v /home/user/app:/var/www/site \
        mobilesnapp/dockbox-hhvm

## Author

MobileSnapp (support@mobilesnapp.com)


## Author

MobileSnapp (support@mobilesnapp.com)

