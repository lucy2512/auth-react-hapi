# Use Node.js image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy source code
COPY . .

# Expose Vite's development server port
EXPOSE 5173

# Start React app in development mode
CMD ["npm", "run", "dev"]
