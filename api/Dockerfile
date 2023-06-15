FROM node:16

WORKDIR /app

COPY ./api/package* ./

RUN npm install 

COPY ./api . 

RUN npm install -g pm2

EXPOSE 3000

CMD pm2 start index.js && tail -f /dev/null
