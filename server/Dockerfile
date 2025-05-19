# Use official Node.js image for server
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy server files
COPY package.json package-lock.json* ./
RUN npm install
COPY . .

# Expose server port
EXPOSE 5000

# Start server
CMD ["node", "index.js"]
