# Під'єднуємо образ пхп, вєрсію з сервером апаче
FROM php:7.2-apache


WORKDIR /var/www/html
COPY . /var/www/html

EXPOSE 80

# -t - title запускаємо білд з тайтлом:
#  docker build -t my-php-app .

# then: docker run -p 8001:80 -d my-php-app
# -d --detach запустить контейнер/проект в фоні, не заважає писати код в консолі

# Урок 6. Будемо пушити папку пхп на докерхаб:
# docker build -t joshkrab/myphp ./php
# docker push joshkrab/myphp:latest

# Після чого удаляємо його, щоб запушити з гіт хаба
# docker image rm joshkrab/myphp
# docker pull joshkrab/myphp
# Запускаємо його - docker run -p 3001:80 --name joshApp joshkrab/myphp