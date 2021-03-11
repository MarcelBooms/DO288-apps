# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

RUN /usr/bin/sed -i 's/Listen 80/Listen 8080/' /etc/httpd/conf/httpd.conf && \
    chgrp -R 0 /etc/httpd && \
    chmod -R g=u /etc/httpd

USER 1001
EXPOSE 8080
