FROM jekyll/jekyll:3.8
RUN apk update && apk add --no-cache supervisor
COPY supervisord.conf /etc/supervisord.conf

WORKDIR /srv/jekyll
CMD ["/usr/bin/supervisord", "-c", "/etc/supervisord.conf"]
# RUN deluser jekyll
# RUN groupadd -r -g 2000 trydirect; useradd -r -u 2000 -g 2000 -m -c "app account" -d /home/trydirect -s /bin/bash trydirect
# RUN chown -R trydirect. /srv/jekyll
