# Use the official Node.js LTS image
FROM node:20-alpine

# (Optional) Update Alpine packages to fix vulnerabilities
RUN apk update && apk upgrade --no-cache

# Set the working directory
WORKDIR /app

# Copy the rest of the application code
COPY . /app

# Install dependencies
RUN npm install

# Expose the application port (change if your app uses a different port)
EXPOSE 80

# Start the application
CMD ["node", "server.js"]