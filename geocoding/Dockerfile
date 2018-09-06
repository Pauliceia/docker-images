FROM node:carbon

WORKDIR /usr/src/geocoding

ENV TZ=America/Sao_Paulo
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

EXPOSE 3000

CMD [ "npm", "run", "docker" ]