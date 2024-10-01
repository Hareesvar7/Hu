# Use an official Node.js image from Docker Hub
FROM node:14

# Create and set the working directory inside the container
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json .

# Install npm dependencies
RUN npm install

# Copy the entire backend directory into the container
COPY . .

# Expose the port that your app will run on
EXPOSE 5000

# Command to run your application
CMD ["npm", "start"]
