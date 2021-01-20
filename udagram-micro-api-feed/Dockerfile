#Use NodeJs base image
FROM node:13


#Create app directory
WORKDIR /usr/src/app

#Copy app dependecies
COPY package*.json ./

#Install app dependecies
RUN npm ci

#Copy app source
COPY . .

#Bind the port the image will run
EXPOSE 8080

#Define docker image behavior at runtime
CMD ["npm", "run", "prod"]
