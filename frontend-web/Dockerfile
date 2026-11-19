# Node.js 24 with Debian Bookworm
FROM node:24-bookworm

# Application directory
WORKDIR /app

# Copy dependency files
COPY package*.json ./

# Install project dependencies
RUN npm ci

# Copy frontend source code
COPY . .

# Vite development port
EXPOSE 5173

# Start Vite development server
CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]
