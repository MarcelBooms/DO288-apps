# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

USER 1001

EXPOSE 8080

ONBUILD sed -i 's/Listen 80/Listen 8080' /etc/httpd/conf/httpd.conf

RUN chgrp -R 0 /etc/httpd && \
    chown -R g=u /etc/httpd
