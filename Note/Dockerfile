# Use a minimal Node.js image as the base
FROM node:18-slim

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json first for efficient caching
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the package.json and package-lock.json files
COPY . .

# Expose the app's port
EXPOSE 4000

# Define the command to run your app
CMD ["node", "index.js"]
