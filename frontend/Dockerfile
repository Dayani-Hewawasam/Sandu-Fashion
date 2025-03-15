# Dockerfile for React client

# Build react client
#alphine is light weighted image
# FROM node:20-alpine  
FROM node

# Working directory be app
WORKDIR /usr/src/app

COPY package*.json ./

###  Installing dependencies
COPY ./node_modules ./node_modules

RUN npm install --verbose
 
# copy local files to app folder
COPY . .

EXPOSE 3000

CMD ["npm","start"]