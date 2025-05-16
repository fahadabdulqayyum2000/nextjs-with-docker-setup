# Base image
FROM node:18-alpine

# Set working directory
WORKDIR /workspace

# Install dependencies
RUN apk add --no-cache bash git

# Copy package.json and lock file
COPY package*.json ./

# Install npm dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Default command
CMD ["npm", "run", "dev"]