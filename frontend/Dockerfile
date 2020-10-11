FROM node:12.19.0-alpine

WORKDIR /app

RUN apk update && \
    apk add git && \
    npm install -g npm@latest && \
    npm install -g @vue/cli

CMD ["/bin/ash"]
