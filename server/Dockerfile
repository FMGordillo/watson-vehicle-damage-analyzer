FROM node:latest

MAINTAINER Facundo Martin Gordillo <famargor@ar.ibm.com>

RUN mkdir -p /usr/app
WORKDIR /usr/app

COPY ["package.json", "/usr/app"]
RUN yarn

EXPOSE 3000

COPY [".", "/usr/app"]
CMD ["npm", "run", "dev"]