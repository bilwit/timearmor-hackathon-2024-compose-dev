FROM node:20-alpine

WORKDIR /var/www/html/timearmor-hackathon-2024

ARG API_PORT
ARG POSTGRES_PASSWORD

ENV TZ America/Los_Angeles
ENV SHELL /bin/ash
ENV API_PORT=$API_PORT
ENV DATABASE_URL=postgres://postgres:$POSTGRES_PASSWORD@timearmor-hackathon-2024-database/postgres

RUN apk add --no-cache --update tzdata \
  ffmpeg \
  git \
  openssh \
  && mkdir -p /var/opt/certs \
  && mkdir -p /root/.ssh \
  && chown -R root:root /root/.ssh \
  && npm i -g npm@latest

EXPOSE $API_PORT