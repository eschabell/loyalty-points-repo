# Wishlist is to move this to RHEL
# FROM http://registry.access.redhat.com/rhscl/nodejs-6-rhel7:6
FROM node:boron

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install app dependencies
COPY package.json /usr/src/app/
RUN npm install

# Bundle app source
COPY . /usr/src/app/

EXPOSE 8080
CMD [ "npm", "start" ]
