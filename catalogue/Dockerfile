FROM node:24.20.0-alpine3.24
# create /app and set the directory to /app
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO_URL="mongodb://mongodb:27017/catalogue" \
    MONGO="true"
CMD ["node", "server.js"]