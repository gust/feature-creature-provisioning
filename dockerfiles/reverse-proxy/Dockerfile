FROM nginx:1.9.12

COPY feature-creature.conf /etc/nginx/conf.d/
COPY dot_htpasswd /etc/nginx/.htpasswd

RUN mkdir /etc/nginx/logs
RUN touch /etc/nginx/logs/feature-creature.access.log

RUN service nginx restart
