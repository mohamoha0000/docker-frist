# Use official Node.js image
FROM node:20

# Create app directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json (if exists)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of your application
COPY . .

# Expose the port your app listens on (change if needed)
EXPOSE 5000

# Start the app
CMD ["node", "index.js"]
