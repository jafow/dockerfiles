FROM node:12.17-buster-slim

ARG APP_USER="appuser"
ENV NODE_ENV "development"

# copy script
COPY bin/ /usr/local/bin/

RUN groupadd -r ${APP_USER} && useradd --no-log-init -r -g ${APP_USER} ${APP_USER}
USER ${APP_USER}

CMD ["node"]
