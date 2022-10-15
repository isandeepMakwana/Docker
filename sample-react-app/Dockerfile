FROM node:alpine3.16
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . .
ENV API_URL=http://api.myapp.com
EXPOSE 3000
RUN addgroup app && adduser -S -G app app
USER app