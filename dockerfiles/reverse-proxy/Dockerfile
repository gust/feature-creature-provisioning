FROM nginx:1.9.12

COPY nginx.conf /etc/nginx/nginx.conf
COPY feature-creature.conf /etc/nginx/conf.d/
COPY dot_htpasswd /etc/nginx/.htpasswd
COPY proxy_params /etc/nginx/proxy_params

RUN mkdir /etc/nginx/logs
RUN touch /etc/nginx/logs/feature-creature.access.log
RUN touch /etc/nginx/logs/feature-creature.error.log

RUN service nginx restart

