# Use an official Node.js image
FROM node:22-alpine

# Create app directory
WORKDIR /app

# Install app dependencies
COPY package*.json ./
RUN npm install

# Copy source code
COPY . .

# Build TypeScript code (if you use a separate build step)
# RUN npm run build 

# Expose the port (e.g., 3001)
EXPOSE 3001

# Start the application
CMD [ "npm", "run", "start" ]
# You'll need to define 'start' in backend/package.json