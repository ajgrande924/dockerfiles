# FROM node:6-alpine
# FROM node:8-alpine
FROM node:10-alpine

# Install app dependencies
ENV NPM_CONFIG_LOGLEVEL warn
RUN apk add --no-cache libc6-compat && \
    npm install pm2 -g

# Show current folder structure in logs
# RUN ls -al -R

# Expose ports
EXPOSE 80 443 43554