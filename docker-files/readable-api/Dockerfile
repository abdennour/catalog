FROM node:boron
MAINTAINER Abdennour TOUMI <http://abdennoor.com>

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
COPY package.json .
# For npm@5 or later, copy package-lock.json as well
# COPY package.json package-lock.json ./

RUN npm install

# Bundle app source
COPY . .

EXPOSE 3010
CMD [ "npm", "start" ]
