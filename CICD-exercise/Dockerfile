FROM node:alpine
RUN apk --no-cache add curl
# Create app directory
WORKDIR /app
COPY ["package*.json", "bin/", "public/", "routes/", "./"]
RUN npm install
# Bundle app source
COPY . .
EXPOSE 3000
CMD [ "npm", "start" ]

