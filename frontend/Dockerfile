FROM node:8

WORKDIR /app/

# Install dependencies
COPY package.json yarn.lock /app/

RUN npm install

# add rest of the client code
COPY . /app/

EXPOSE 3000

CMD npm start

