FROM openjdk:14-jdk-alpine3.10

RUN apk update && \
    apk add \
    bash

RUN wget https://github.com/partiql/partiql-lang-kotlin/releases/download/v0.1.0-alpha/partiql-cli-0.1.0.tgz
RUN mkdir /bin/partiql && tar -xvzf partiql-cli-0.1.0.tgz -C /bin/partiql --strip-components 1
RUN ln -s /bin/partiql/bin/partiql /usr/local/bin/partiql

