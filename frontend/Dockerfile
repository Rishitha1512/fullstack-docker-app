# Use Node base image
FROM node:14-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json first
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy frontend source code
COPY . .

# Expose React app port
EXPOSE 3000

# Start React app
CMD ["npm", "start"]
