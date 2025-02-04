FROM node:21-alpine

# Defined the working directory
WORKDIR /app

# Copy the files
COPY . .

RUN npm install


#EXPOSE port 80
EXPOSE 80

# Start App
CMD ["node", "server.js"]
