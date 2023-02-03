FROM node:19.6.0-alpine3.16

# Create user
# RUN addgroup app && adduser -S -G app app

# USER app

# working directory
WORKDIR /app

# Copy content from current directory to working directory
COPY package*.json .
# Run commands
RUN npm install

COPY . .

# it adds URL or compressed file
# ADD URL .

# Env variables

ENV API_URL=http://api.myapp.com

EXPOSE 3001:3000

CMD npm start