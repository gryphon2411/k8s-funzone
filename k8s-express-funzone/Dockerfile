# Use the official Node.js runtime as the base image
FROM node:18

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the rest of the app source code to the container
COPY . .

# Expose the port on which the index app will run
EXPOSE 3000

# Expose the port on which the uselessfacts app will run
EXPOSE 4000

# Define the command to run the app when the container starts
CMD [ "node", "index.js" ]
