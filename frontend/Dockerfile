FROM node:17-alpine

# Set working directory
WORKDIR /app

# Copy package.json file to working directory
COPY ./package.json /app/package.json

# copy other files/folders to working directory
COPY . /app

# Same as npm install
RUN npm install
RUN npm run build

# expose port 3000
EXPOSE 3000

CMD [ "npm", "start" ]
