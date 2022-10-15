FROM node:14.4-alpine3.11
RUN addgroup app && adduser -S -G app app
USER app
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . .
ENV API_URL=http://api.myapp.com
EXPOSE 3000
CMD ["npm","start"]
