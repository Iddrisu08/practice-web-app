# Use an official Ubuntu 14.04 base image
FROM ubuntu:14.04

# Update package list and install Apache HTTP Server
RUN apt-get update && apt-get install -y apache2 apache2-utils && apt-get clean

# Copy index.html into Apache document root
COPY index.html /var/www/html/

# Start Apache HTTP Server in the foreground
CMD ["apache2ctl", "-D", "FOREGROUND"]

