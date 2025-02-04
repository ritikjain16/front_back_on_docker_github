# Use Node.js image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy rest of the backend files
COPY . .

# Expose backend API port
EXPOSE 5000

# Start the backend server
CMD ["node", "index.js"]
