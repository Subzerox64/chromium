FROM alpine:3.12
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY package.json /usr/src/app
RUN apk add --no-cache npm nodejs coreutils
RUN npm init
RUN npm i
COPY index.js /usr/src/app
COPY run.sh /usr/src/app
