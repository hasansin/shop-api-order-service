#get node base image from Dockerfile
FROM node:16-alpine

#working directory
WORKDIR /app

#
COPY package.json .

#install packages
RUN npm install

# copy current directory files to work directory
COPY . .

ENV PORT 5000

EXPOSE $PORT

CMD ["npm","start"]

