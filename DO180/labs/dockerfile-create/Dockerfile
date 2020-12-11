FROM ubi7/ubi:7.7

MAINTAINER Klaus Schwartz <Klaus-Juergen.Schwartz@deutschebahn.com>

LABEL description="A custom Apahe container based on UBI 7"

RUN yum install -y httpd && \
    yum clean all

RUN echo "Hello from Dockerfile" > /usr/share/httpd/noindex/index.html

EXPOSE 80

ENTRYPOINT ["httpd", "-D", "FOREGROUND"]




