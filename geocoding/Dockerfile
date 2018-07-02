FROM node:carbon

WORKDIR /usr/src/geocoding

COPY ./api/package*.json ./

RUN npm install -g express-generator@4.13.4
RUN npm install -g supervisor@0.11.0
RUN npm install

ENV PORT=3000

COPY ./api .

EXPOSE 3000

CMD [ "npm", "start" ]