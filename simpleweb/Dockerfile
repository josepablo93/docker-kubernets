# Specify a base image
FROM node:lts-alpine

# Set the working directory
WORKDIR /usr/app

# Copy dependencies changes to the
# working directoy in the container
COPY ./package.json ./
# Install the dependencies if there was any modification
RUN npm install
# Copy the rest of the files
COPY ./ ./

# Default command
CMD ["npm", "start"]
