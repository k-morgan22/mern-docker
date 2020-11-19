FROM node:14-alpine

# Create App Directory
WORKDIR /app

# Install Dependencies
COPY package.json yarn.lock ./

RUN yarn install

# Copy app source code
COPY . .

# Expose ports
EXPOSE 3001

CMD ["yarn","start"]