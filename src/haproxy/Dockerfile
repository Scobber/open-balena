FROM haproxy:2.9-alpine

VOLUME [ "/certs" ]

USER root
RUN sudo apk add --update inotify-tools
USER haproxy

COPY haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg
COPY start-haproxy.sh /start-haproxy

CMD /start-haproxy
