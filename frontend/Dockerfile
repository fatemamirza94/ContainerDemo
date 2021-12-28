# Pull node image based on node 16.13.1

FROM node:16.13.1


# Set working directory

WORKDIR /frontend


# Copy package files from React app to working directory

COPY ./package.json ./
COPY ./package-lock.json ./


# Copy src and public folder from React app to working directory

COPY ./src ./src
COPY ./public ./public


# Expose ports

Expose 3000


# install app dependencies

RUN npm install


# Start the React app

CMD ["npm", "start"]

