FROM node:18-alpine
WORKDIR /app
COPY index.js .
RUN npm init -y && npm install express mongoose
CMD ["node", "index.js"]
 