FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install 

COPY . . 

EXPOSE 80


#This code does not work since it creates a hidden folder that stop existing at the time of the deletion of the container 
#VOLUME ["/app/feedback"] #Path inside of the container, that should be mapped outside of the container, it is feedback as per the code in node

#VOLUME ["/app/node_modules"] # this is to keep the node_modules inside of the container and avoid missing dependencies



CMD ["npm", "start"]