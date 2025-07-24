# tells docker how to build the backend Node.js container

FROM node:18 
# Base image with Node.js v18 installed

WORKDIR /usr/src/app 
# the directory in which all the following commands will run

COPY package*.json ./
RUN npm install
# copies package files and installs dependencies

COPY . .
# copies the rest of the app's code

CMD ["node", "index.js"]
# starts the app using Node.js
