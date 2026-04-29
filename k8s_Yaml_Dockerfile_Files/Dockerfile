# Step 1: Use an official Node.js base image
FROM node:18-alpine

# Step 2: Set the working directory in the container
WORKDIR /app

# Step 3: Copy package.json
COPY package*.json ./

# Step 4: Install the app dependencies
RUN npm install

# Step 5: Copy the rest of the application code
COPY . .

# Step 6: Expose the port the app runs on (assumed 3000)
EXPOSE 3000

# Step 7: Define the command to start the app
CMD ["npm", "start"]