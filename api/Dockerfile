# first layer
FROM node:17-alpine

# specify working directory
WORKDIR /app

# copy package json
COPY package.json .

# run at build time
RUN npm install

# copy relative files to the working directory
COPY . .

# expose a port to container
EXPOSE 4000

# run on container
CMD ["node", "app.js"]


# build:
# docker build -t myapp .