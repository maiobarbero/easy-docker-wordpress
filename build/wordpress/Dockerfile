ARG WORDPRESS_VERSION=latest
FROM wordpress:${WORDPRESS_VERSION}

RUN apt-get update && apt-get install -y default-mysql-client

# Uncomment if you want to copy your folder into the container
#
# COPY ./custom-theme /var/www/html/wp-content/themes/custom-theme
# COPY ./custom-plugins /var/www/html/wp-content/plugins/custom-plugins

# Copy the custom php.ini file to configure PHP settings
COPY ./config/php.conf.ini /usr/local/etc/php/php.ini

# Set authorizations
RUN chown -R www-data:www-data /var/www/html/