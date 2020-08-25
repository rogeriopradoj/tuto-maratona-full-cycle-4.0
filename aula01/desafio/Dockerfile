FROM nginx:alpine

RUN chmod -R a+w /var/cache/nginx/ \
    && touch /var/run/nginx.pid \
    && chmod a+w /var/run/nginx.pid \
    && rm /etc/nginx/conf.d/*

COPY eu-sou-full-cycle.conf /etc/nginx/conf.d/
EXPOSE 8080
USER nginx