# 1. For build React app
FROM node:lts AS development

# Set working directory
WORKDIR /app

# 
COPY package.json /app/package.json

# Same as npm install
RUN npm i

COPY . /app

ENV I=true
ENV PORT=3000

CMD [ "npm", "start" ]

FROM development AS build

RUN npm run build