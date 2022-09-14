FROM node:16

  RUN npm install -g nodemon

WORKDIR /home/workspace

  COPY package.json .
  RUN npm install --omit=dev

WORKDIR /home/workspace/apps

  CMD [ "nodemon", "my-service/main.js" ]