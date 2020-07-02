# base image
FROM node:13

# set working directory within container filesystem
WORKDIR /app

# install and cache app dependencies
COPY package*.json ./
RUN npm install

# Copy whole backend app source
COPY . .

# start app
CMD [ "node", "server.js" ]