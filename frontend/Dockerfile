FROM node:alpine

WORKDIR /app

COPY react-app/package.json /app

RUN npm install

COPY react-app /app

CMD ["npm", "run", "start"]
