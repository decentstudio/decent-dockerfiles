FROM node:alpine

LABEL maintainer="cjbarre@gmail.com" \
      org="DecentStudio"             \
      version="1.0"                  \
      app="node-environment"         \
      description="Use this container to build/run/test nodejs code."

RUN apk update && apk add vim tmux

VOLUME ["/code/"]

WORKDIR /code

ENTRYPOINT ["sh"]
