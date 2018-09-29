FROM node:8.12

RUN npm i -g gulp-cli
RUN apt-get update
RUN apt-get install -y graphicsmagick \
    graphicsmagick-imagemagick-compat \
    && apt-get clean
RUN rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["gulp"]