# Base the image on the official Node.js runtime
FROM node:14

# Set the working directory within the container
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json files
COPY package*.json ./

# Install the Node.js dependencies
RUN npm install

# Copy the remaining application code
COPY . .

# Expose the port where the application runs
EXPOSE 3000

# Specify the command to start the application
CMD ["npm", "start"]
