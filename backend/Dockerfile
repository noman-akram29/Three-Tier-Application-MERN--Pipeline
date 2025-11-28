# Base image for backend
FROM node:21-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install required dependencies
RUN npm install

# RUN npm run tests

# Install nodemon for hot reload
RUN npm install -g nodemon

# Copy the rest of the application code to the working directory
COPY . .

COPY .env.sample .env
# Expose the port the app runs on
EXPOSE 5000

# Command to start the backend server
CMD ["npm", "start"]
