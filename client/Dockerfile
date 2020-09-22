###############################################
#     Dockerfile to build the backend         #
###############################################

# Base image is node
FROM node:14.11.0-alpine3.10

# Author: Maureen
LABEL maintainer="Maureen Sitienei<mstienei@gmail.com>"

# Create Working directory
WORKDIR /opt/yolo/client

# Copy the backend directory from the Docker host to the filesystem of the new image(working directory)
COPY . .

COPY package*.json ./

# Expose port for the process to listen to 
EXPOSE 3000

# Install npm package
RUN npm install

# Run app
# Set command for CMD
CMD ["npm", "start"]