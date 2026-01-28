FROM node:18-alpine

WORKDIR /app

# Copy dependency files first
COPY package*.json ./

RUN npm install --production

# Copy backend source
COPY . .

EXPOSE 8080

CMD ["node", "server.js"]
