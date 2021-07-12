FROM node:14

# Create app directory
WORKDIR /code

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)

RUN npm install -g @angular/cli && npm install

EXPOSE 4200

COPY package*.json ./code



# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY . .


CMD ["npm", "start"]