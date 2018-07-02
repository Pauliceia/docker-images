FROM node:carbon

WORKDIR /usr/src/geoserver-rest

COPY ./api/package*.json ./

RUN npm install --only=production

COPY ./api .

EXPOSE 3002

CMD [ "npm", "run", "prod" ]