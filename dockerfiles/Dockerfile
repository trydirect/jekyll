FROM jekyll/jekyll:3.8
RUN deluser jekyll
RUN groupadd -r -g 2000 jekyll; useradd -r -u 2000 -g 2000 -m -c "app account" -d /home/jekyll -s /bin/bash jekyll
RUN chown -R jekyll. /srv/jekyll
USER jekyll
WORKDIR /srv/jekyll
