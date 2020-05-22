# Use NodeJS base image
FROM node:12.6.0

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies by copying
# package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm i -g @ionic/cli
RUN npm i

# Copy app source
COPY . .

# Bind the port that the image will run on
EXPOSE 8100

# Define the Docker image's behavior at runtime
CMD ["ionic", "serve", "--external", "--host", "0.0.0.0", "--disableHostCheck", "true"]
