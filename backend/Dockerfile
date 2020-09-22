###############################################
#     Dockerfile to build the backend         #
###############################################

# Base image is node
FROM node:14.11.0-alpine3.10

# Author: Maureen
LABEL maintainer="Maureen Sitienei<mstienei@gmail.com>"

# Create Working directory
WORKDIR /opt/backend

# Copy the backend directory from the Docker host to the filesystem of the new image(working directory)
COPY . .

COPY package*.json ./

# Expose port for the process to listen to 
EXPOSE 5000

# Set command for CMD
CMD ["node", "server.js"]