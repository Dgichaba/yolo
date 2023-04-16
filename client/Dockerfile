FROM node:18-alpine as build

RUN mkdir /app

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

RUN npm install -g serve 

FROM gcr.io/distroless/nodejs18-debian11 

COPY --from=build /app /app 

WORKDIR /app 

EXPOSE 3000

CMD [ "npm" , "start" ]