#Base image
FROM node:lts-alpine

#install dependencies
#if not created then it will create a file
WORKDIR /usr/app/

# copy package.json from build context to container context
COPY ./package.json ./
#run the commands
RUN npm install
#copy everything
COPY ./ ./
#Default command
CMD ["npm", "start"]