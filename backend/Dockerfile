# Stage 1
FROM node:20-alpine AS build

WORKDIR /app
COPY package*.json ./
RUN npm install

COPY . .

# Stage 2
FROM node:20-alpine

WORKDIR /app 

COPY --from=build /app/package*.json ./
RUN npm install --omit=dev

COPY --from=build /app .

EXPOSE 5000


CMD ["node", "server.js"]