# Use Node.js 19 image
FROM node:19

# Set working directory
WORKDIR /app

# Copy package.json and yarn.lock
COPY package.json yarn.lock ./

# Install dependencies
RUN yarn install

# Copy the rest of the application code
COPY . .

# Copy the .env file
COPY .env .env

# Expose the necessary port
EXPOSE 3000

# Start the application
CMD ["yarn", "start"]
