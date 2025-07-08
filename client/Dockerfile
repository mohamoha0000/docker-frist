# Use Node.js image
FROM node:20

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of your React app
COPY . .

# Expose the port React dev server will run on
EXPOSE 453

# Set environment variable to change port
ENV PORT=453

# Start React app (development mode)
CMD ["npm", "start"]
