FROM node:14 AS react-builder

WORKDIR /app/react

# Copy package.json and package-lock.json to the container
COPY . .

# Install app dependencies
RUN npm install

# Build the React app
RUN npm run build

# Make port 3000 available to the world outside this container
EXPOSE 3000

# Run start script
CMD ["npm", "start"]