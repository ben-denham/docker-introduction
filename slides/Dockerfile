FROM node:6

RUN wget -O /usr/local/bin/dumb-init https://github.com/Yelp/dumb-init/releases/download/v1.2.0/dumb-init_1.2.0_amd64
RUN chmod +x /usr/local/bin/dumb-init

WORKDIR /opt/docker-intro
COPY . /opt/docker-intro/

RUN npm i

EXPOSE 8000

CMD ["/usr/local/bin/dumb-init", "npm", "start"]
