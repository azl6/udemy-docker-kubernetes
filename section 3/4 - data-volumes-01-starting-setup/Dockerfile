FROM node

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 80

CMD ["node", "server.js"]

#For this practice, I've learned that the '-v' flag can set us a named volume, which can be used to retrieve data,
#even if the container dies. 


