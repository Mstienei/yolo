###############################################
#     Dockerfile to build the backend         #
###############################################

# Base image is node.js
FROM node:14.11.0-alpine3.10

# Author: Maureen
LABEL maintainer="Maureen Sitienei<mstienei@gmail.com>"

# Create Working directory
WORKDIR /opt/backend

COPY . .

COPY package*.json ./

EXPOSE 5000

# Set command for CMD
CMD ["node", "server.js"]