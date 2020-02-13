# Define the PHP image to use - You may select a different image per your needs
# Check the online doc for more details and available options
FROM php:7.4-apache

# Populate the image www file from the local fs
COPY wordpress/ /var/www/html
RUN chmod -R 755 /var/www/html

# make a copy of the deployment (needed in case of kubernetes deployment to
# populate/init the created persistent volumes)
RUN mkdir ~/initial-deployment
RUN cp -R /var/www/html/* ~/initial-deployment
RUN chmod -R 755 ~/initial-deployment

# Listen on port 80 (http)
EXPOSE 80