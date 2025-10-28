# Use Node 22 Alpine
FROM node:22-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the app
COPY . .

# Build the Next.js app
RUN npm run build

# Expose the port Next.js will use
EXPOSE 3000

# Start the app in production mode
CMD ["npm", "start"]
