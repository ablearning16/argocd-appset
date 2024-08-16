# Use Node.js LTS as base image
FROM node:14

# Set the working directory
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json files
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the application
COPY . .

# Expose the application port 
EXPOSE 3000

# Start the application
CMD ["npm", "start"]