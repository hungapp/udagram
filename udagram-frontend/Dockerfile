## Build
# Use NodeJS base image
FROM node:12.6.0
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

RUN npm i -g @ionic/cli
RUN npm ci

# Bundle app source
COPY . .
RUN ionic build


#COPY www /usr/share/nginx/html
COPY /usr/src/app/www /usr/share/nginx/html
