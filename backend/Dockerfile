FROM node:14
WORKDIR /app
COPY package*.json ./
RUN npm install
RUN npm install -g sequelize-cli
RUN npm install mysql2
RUN npm install bcrypt
RUN npm install express
RUN npm install express-sslify
RUN npm install jsonwebtoken
RUN npm install moment
RUN npm install multer
RUN npm install path
RUN npm install sequelize
RUN npm install socket.io
RUN npm install web-push
COPY . .
EXPOSE 3000
#CMD [ "npm", "start" ]
CMD sequelize db:create && sequelize db:migrate && npm start

