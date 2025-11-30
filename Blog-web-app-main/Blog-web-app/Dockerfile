# 1) Use Node.js base image
FROM node:18-alpine

# 2) Set working directory inside container
WORKDIR /app

# 3) Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# 4) Copy project files
COPY . .

# 5) Expose the port your app uses (change if not 3000)
EXPOSE 3000

# 6) Command to start the app
CMD ["node", "index.js"]
