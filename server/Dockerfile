FROM node:16

# Create app directory
WORKDIR /usr/src/app

# install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copies
# where available (npm@5+)
COPY package*.json ./

RUN npm install
# If you are building code for pruduction
# RUN npm ci --only=production

# Bundle app source
COPY . .

EXPOSE 7777
CMD ["npm", "run", "start"]



