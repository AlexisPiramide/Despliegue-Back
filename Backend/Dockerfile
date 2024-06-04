FROM node:latest

WORKDIR /back

RUN npm install -g nodemon --save-dev
RUN npm install -g ts-node

RUN git clone https://github.com/AlexisPiramide/Aplicacion-Tiempo-BackEnd .

RUN npm install

CMD ["npm", "run", "dev"]