FROM node:8

MAINTAINER Stephen Lewis

# @see https://github.com/nodejs/docker-node/blob/master/docs/BestPractices.md#global-npm-dependencies
ENV NPM_CONFIG_PREFIX=/home/node/.npm-global
ENV PATH=$PATH:/home/node/.npm-global/bin

# @see https://github.com/nodejs/docker-node/blob/master/docs/BestPractices.md#non-root-user
USER node

WORKDIR /home/node/app

RUN npm install -g gulp

# Now that we've changed the global path, we need to reinstall yarn globally
RUN npm install -g yarn

VOLUME ["/home/node/app"]

CMD ["gulp", "watch"]
