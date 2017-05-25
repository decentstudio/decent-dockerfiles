FROM node:alpine

LABEL maintainer="cjbarre@gmail.com" \
      org="DecentStudio"             \
      version="1.0"                  \
      app="clojure-environment"      \
      description="Use this container to build/run/test Clojure code."

ENV LEIN_ROOT=true

RUN apk update && apk add wget ca-certificates bash vim tmux openjdk8

RUN wget "https://raw.githubusercontent.com/technomancy/leiningen/stable/bin/lein" -O /bin/lein \
    && chmod a+x /bin/lein \
    && lein

WORKDIR $HOME/root

COPY .vimrc .vimrc

VOLUME ["/code/"]

WORKDIR /code

ENTRYPOINT ["sh"]
