ARG PHP_VERSION=8.2
FROM php:${PHP_VERSION}-cli-alpine

ARG PDEPEND_VERSION=2.15.1
ARG PDEPEND_DOWNLOAD_SHA256=d14701de2c16ba2fdec40b6c73f8c6ba03a60c93b619493ce80a23d161a129d6

COPY ./files/pdepend-wrapper.sh /usr/local/bin/pdepend

RUN apk --update --no-cache --virtual .download add curl \
    && curl -L --fail -o /usr/local/bin/pdepend.phar \
        "https://github.com/pdepend/pdepend/releases/download/${PDEPEND_VERSION}/pdepend.phar" \
    && echo "$PDEPEND_DOWNLOAD_SHA256  /usr/local/bin/pdepend.phar" > /usr/local/bin/pdepend.sha256 \
    && sha256sum -w -c /usr/local/bin/pdepend.sha256 \
    && rm -f /usr/local/bin/pdepend.sha256 \
    && apk del .download \
    \
    && chmod +x /usr/local/bin/pdepend

ENTRYPOINT ["/usr/local/bin/pdepend"]
