FROM keitwb/calibre-base

MAINTAINER Ben Keith <keitwb@gmail.com>

ADD run-server.sh /opt/run-server.sh
RUN chmod +x /opt/run-server.sh

RUN touch /var/log/calibre.log && chown calibre:calibre /var/log/calibre.log

USER calibre
EXPOSE 8080

ENTRYPOINT ["/opt/run-server.sh"]
