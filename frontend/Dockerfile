# Use an official Node.js image
FROM node:14

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json .

# Install npm dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Build the application for production
RUN npm run build

# Expose the port the app will run on
EXPOSE 3000

# Command to run your application (using serve package to serve the build)
CMD ["npx", "serve", "-s", "build"]
