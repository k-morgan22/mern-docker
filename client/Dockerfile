FROM node:latest

# Create App Directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install Dependencies
COPY package.json yarn.lock ./

RUN yarn install

# Copy app source code
COPY . .

# Expose ports
EXPOSE 3000

CMD ["yarn","start"]