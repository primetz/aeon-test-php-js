ARG MYSQL_VERSION

FROM mysql:${MYSQL_VERSION}

ARG USER_ID
ARG GROUP_ID

RUN usermod -u ${USER_ID} mysql && \
    groupmod -g ${GROUP_ID} mysql \
