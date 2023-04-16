FROM  node:13.12.0-alpine as backend

RUN mkdir /app

WORKDIR /app

COPY package * .json ./

RUN npm install

COPY . /app/

EXPOSE 5000

CMD ["npm" , "start"]