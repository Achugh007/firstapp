# Use the official Node.js runtime as the base image
FROM node:18

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json (if available)
# COPY package*.json ./
# COPY backend/package*.json ./

# Install dependencies
RUN npm install

# If you are building production
# RUN npm ci --only=production

# Bundle app source
COPY . .

# Expose the port your app runs on (replace 8080 with the actual port)
EXPOSE 3000 

# Define the command to run your app
CMD [ "npm", "start" ] 
