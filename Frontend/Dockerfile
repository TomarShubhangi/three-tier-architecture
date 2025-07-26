# Use official Node.js image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Install a simple HTTP server globally
RUN npm install -g http-server

# Copy your static files (index.html, etc.) to /app
COPY . .

# Expose the port http-server runs on
EXPOSE 8081

# Start the static file server
CMD ["http-server", "-p", "8081"]

