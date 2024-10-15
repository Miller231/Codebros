# Use the official Node.js image
FROM node:16

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the project files
COPY . .

# Build the project
RUN npm run build

# Serve the project
EXPOSE 8080
CMD ["npm", "run", "serve"]
