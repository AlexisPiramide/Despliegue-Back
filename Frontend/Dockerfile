FROM node:latest

RUN apt update && apt install -y apache2  

WORKDIR /app

RUN git clone -b front-timepo https://github.com/AlexisPiramide/front-tiempo/ .

RUN npm install
RUN npm run build

RUN cp -r dist/* /var/www/html/

CMD ["apachectl", "-D", "FOREGROUND"]