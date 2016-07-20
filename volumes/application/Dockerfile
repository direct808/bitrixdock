FROM debian:jessie

MAINTAINER Vitams <vmpartner@gmail.com>

RUN apt-get update && apt-get install -y --force-yes \
        wget

WORKDIR /var/www/site

RUN cd /var/www/site && wget 'http://www.1c-bitrix.ru/download/scripts/bitrixsetup.php'

RUN chown -R www-data:www-data /var/www/site/
RUN chmod -R 775 /var/www/site

CMD ["true"]
